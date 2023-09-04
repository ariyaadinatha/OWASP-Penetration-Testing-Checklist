# OWASP Mobile Application Security Testing Checklist

## Table of Contents

* [Static Analysis](#Static)
* [Dynamic and Runtime Analysis](#Dynamic)
* [Secure Transmission](#Transmission)
* [Server Side - Webservices and API](#Server)

-------
### <a name="Static">Static Analysis</a>

- [ ] Reverse Engineering the Application Code (Code Obfuscating Checking)
- [ ] Information leakage/Hardcoded credential in the binaries 
- [ ] Unauthorized Code Modification
- [ ] Misuse of App permissions
- [ ] Insecure version of OS Installation Allowed
- [ ] Abusing Android Components through IPC intents ("exported" and "intent-filter")
- [ ] Unrestricted Backup file
- [ ] Cryptographic Based Storage Strength
- [ ] Poor key management process
- [ ] Use of custom encryption protocols
- [ ] Debuggable Application


### <a name="Dynamic">Dynamic and Runtime Analysis</a>

- [ ] Misuse of Keychain , Touch ID and other security related controls
- [ ] Minimum Device Security Requirements absent
- [ ] Unencrypted Database files
- [ ] Insecure Shared Storage
- [ ] Insecure Application Data Storage
- [ ] Information Disclosure through Logcat/Apple System Log (ASL)
- [ ] Application Backgrounding (Screenshot)
- [ ] Copy/Paste Buffer Caching
- [ ] Keyboard Press Caching
- [ ] Unrestricted Backup file
- [ ] Remember Credentials Functionality (Persistent authentication)
- [ ] Client Side Based Authentication Flaws
- [ ] Client Side Authorization Breaches
- [ ] Content Providers: SQL Injection and Local File Inclusion
- [ ] Broadcast Receiver
- [ ] Service component
- [ ] Insufficient WebView hardening
- [ ] Injection (SQLite Injection, XML Injection)
- [ ] Local File Inclusion through Webviews
- [ ] Abusing URL schemes or Deeplinks
- [ ] Sensitive Information Masking
- [ ] Runtime Manipulation
- [ ] Rooted or Jail-broken device checking
- [ ] Passwords/ Connection String disclosure
- [ ] Hidden and Unscrutinised functionalities


### <a name="Transmission">Secure Transmission</a>

- [ ] Insecure Transport Layer Protocols
- [ ] Use of Insecure and Deprecated algorithms
- [ ] Use of Disabling certificate validation
- [ ] SSL pinning Implementation
- [ ] End-to-end encryption


### <a name="Server">Server Side - Webservices and API</a>

- [ ] Excessive port opened at Firewall
- [ ] Default credentials on Application Server
- [ ] Weak password policy Implementation
- [ ] Exposure of Webservices through WSDL document
- [ ] Security Misconfiguration on Server API
- [ ] Security Patching on Server API
- [ ] Input validation on API
- [ ] Information Exposure through API response message
- [ ] Control of interaction frequency on API (Replay Attack)
- [ ] Session invalidation on Backend
- [ ] Session Timeout Protection
- [ ] Cookie Rotation
- [ ] Multiple concurrent logins
- [ ] Exposing Device Specific Identifiers in Attacker Visible Elements
- [ ] Token/Session Creation and handling
- [ ] Insecure Direct Object references
- [ ] Missing function level access control
- [ ] Bypassing business logic flaws

Source: [MobileApp-Pentest-Cheatsheet](https://github.com/tanprathan/MobileApp-Pentest-Cheatsheet/tree/master)
