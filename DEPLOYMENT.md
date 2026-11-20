# Controlled Render deployment

1. Deploy as a Render Static Site from branch main, publish directory public, build command `echo Static site ready`, auto-deploy off.
2. Test /, /games/, /reaction-rush/, /reaction-rush/privacy/ and /contact/ at the generated onrender.com hostname, including mobile rendering.
3. Add the apex domain maurointeractive.com in Render custom domains and obtain actual DNS values.
4. In Squarespace, replace only the existing Squarespace web-hosting records (four apex A records, www CNAME and incompatible HTTPS/SVCB records if directed after review).
5. Preserve Google Workspace MX smtp.google.com, SPF include:_spf.google.com, DKIM google._domainkey, all verification and DMARC records, the domainconnect record and the nameservers.
6. Confirm HTTPS, privacy URL with/without trailing slash, www behavior, and all four mailboxes.
7. Enter https://maurointeractive.com/reaction-rush/privacy in Google Play Console; verify Data Safety declarations and in-app link.

No DNS change is part of merely committing this repository. Do not put credentials or the Android upload keystore in this repository.
