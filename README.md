# Email-Verifier
Validates emails, including cross-checking TLD with ICANN

To use, simply add this in your header:

    <script src="emailverifier.js"></script>

To validate an email using JavaScript, use:

    if (validateEmail(yourtextbox.value)) //Valid Email

A simple demo that alerts the user whether the email is Valid or Invalid:

    alert((validateEmail(yourtextbox.value)?"V":"Inv")+"alid");


Some example valid email addresses:
    foo.bar@gmail.com         (Standard email)
    booo000oood@yahoo.jp      (Japan TLD)
    boss@nick.digital         (DIGITAL TLD)
    w@yxz.us                  (US TLD)
Some example invalid email addresses:
    extra-dot@typo..com       (Extra .)
    wrong@tld.yippy           (Invalid TLD)
    starwars-at-at@@rocks.co  (Extra @)
    fail.@fail.fail           (Touching .@)
