# Email-Verifier
Validates emails, including cross-checking TLD with ICANN

To use, simply add this in your header:

    <script src="emailverifier.js"></script>

To validate an email using JavaScript, use:

    if (validateEmail(yourtextbox.value)) //Valid Email

A simple demo that alerts the user whether the email is Valid or Invalid:

    alert((validateEmail(yourtextbox.value)?"V":"Inv")+"alid");


<table>
	<tr><td colspan=2><b>Some example valid email addresses:</b></td></tr>
	<tr><td>foo.bar@gmail.com</td><td>Standard email</td></tr>
    <tr><td>booo000oood@yahoo.jp</td><td>Japan TLD</td></tr>
    <tr><td>boss@nick.digital</td><td>DIGITAL TLD</td></tr>
    <tr><td>w@yxz.us</td><td>US TLD</td></tr>
</table>

<table>
<tr><td colspan=2><b>Some example invalid email addresses:</b></td></tr>
    <tr><td>extra-dot@typo..com</td><td>Extra .</td></tr>
    <tr><td>wrong@tld.yippy</td><td>Invalid TLD</td></tr>
    <tr><td>starwars-at-at@@rocks.co</td><td>Extra @</td></tr>
    <tr><td>fail.@fail.fail</td><td>Touching .@</td></tr>
</table>
