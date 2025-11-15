# Blog (TryHackMe) — Writeup

A full walkthrough of the **Blog** room from TryHackMe.  
Main moves:
- WordPress enumeration with WPScan  
- Bruteforce login → logged into WP Admin  
- WordPress 5.0 image-crop RCE (ExploitDB + Metasploit)  
- Grab wp-config → retrieve DB creds  
- Privilege escalation via a custom SUID binary (`checker`) that trusts the `admin` environment variable  
- Root shell gained
