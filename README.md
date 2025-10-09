# Group-2-Mineral-Dashboard
Pseudocode
FUNCTION login(username, password):
    READ user_data FROM users.json
    FIND user WHERE user.username == username
    IF user IS FOUND:
        IF user.password_hash MATCHES password_hash:
            SET session.user_role = user.role
            REDIRECT TO dashboard
        ELSE:
            DISPLAY "Invalid password"
        END IF
    ELSE:
        DISPLAY "User not found"
    END IF
END FUNCTION
