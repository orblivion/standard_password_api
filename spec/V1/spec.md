# API

* Format: Json
* Protocol: HTTPS
* Root URL: /standard_pasword_api/V1/

## Info: /

Accepts:

    GET HEAD

Input:

    (none)

Returns:

    info: ""

## Change Password: /change_password/

Accepts:

    POST

Input:

    old_password: <string>

    new_password: <string>

Output:

    success: "true"|"false"

    error: "authentication"|"password_format"

    password_specifications: <string>

        * Ex - "Password should have at least 8 characters, including one digit and one symbol."
        * Free form
        * Complete sentence.
        * Useful for a user dialog

## Check Password: /check_password/

    TODO

# Client Implementation Requirements

* Confirm the certificate of the site before making an HTTPS request to it.
* Keep any internet-facing code in a different *process* than what has access to the in-memory decrypted password database.
* Check that the site claims to implent this version of the API before posting any sensitive information to it.
