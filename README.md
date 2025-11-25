# Modelo-de-usu-rio-
@Entity
public class Usuario {
    @Id @GeneratedValue
    private Long id;

    private String email;
    private String senha;

    @Enumerated(EnumType.STRING)
    private Role role;
}
public enum Role {
    ROLE_ADMIN,
    ROLE_USER,
    ROLE_VENDEDOR
}
