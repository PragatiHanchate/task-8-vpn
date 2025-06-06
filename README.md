# task-8-vpn┌──(kali㉿kali)-[~]
└─$ sudo apt update                 
[sudo] password for kali: 
Hit:1 http://http.kali.org/kali kali-rolling InRelease
Hit:2 https://repo.protonvpn.com/debian stable InRelease
1696 packages can be upgraded. Run 'apt list --upgradable' to see them.
Warning: http://http.kali.org/kali/dists/kali-rolling/InRelease: Key is stored in legacy trusted.gpg keyring (/etc/apt/trusted.gpg), see the DEPRECATION section in apt-key(8) for details.
Notice: Repository 'Kali Linux' changed its 'non-free component' value from 'non-free' to 'non-free non-free-firmware'
Notice: More information about this can be found online at: https://www.kali.org/blog/non-free-firmware-transition/
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ sudo apt install -y nodejs npm
nodejs is already the newest version (20.19.2+dfsg-1).
npm is already the newest version (9.2.0~ds1-3).
The following packages were automatically installed and are no longer required:
  libpython3.12-dev  python3.12  python3.12-dev  python3.12-minimal  python3.12-venv
Use 'sudo apt autoremove' to remove them.

Summary:
  Upgrading: 0, Installing: 0, Removing: 0, Not Upgrading: 1696
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ node -v         
v20.19.2
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ npm -v 
9.2.0
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ sudo npm install -g proton-cli

changed 64 packages in 5s

2 packages are looking for funding
  run `npm fund` for details
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ sudo npm install -g proton-cli --unsafe-perm+true

changed 64 packages in 923ms

2 packages are looking for funding
  run `npm fund` for details
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ which proton-cli
proton-cli not found
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ 
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ npm bin -g
Unknown command: "bin"

To see a list of supported npm commands, run:
  npm help
                                                                                                                    
┌──(kali㉿kali)-[~]
└─$ cd Downloads         
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ ls
Nessus-10.8.4-debian10_amd64.deb
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ curl -fsSl https://deb.nodesource.com/setup_16.x | sudo -E bash -

================================================================================
================================================================================

                              DEPRECATION WARNING                            

     Node.js 16.x is no longer actively supported!

  You will not receive security or critical stability updates for this version.

  You should migrate to a supported version of Node.js as soon as possible.
  Use the installation script that corresponds to the version of Node.js you
  wish to install. e.g.
  
   * https://deb.nodesource.com/setup_16.x — Node.js 16 "Gallium" (deprecated)
   * https://deb.nodesource.com/setup_18.x — Node.js 18 "Hydrogen" (Maintenance)
   * https://deb.nodesource.com/setup_19.x — Node.js 19 "Nineteen" (deprecated)
   * https://deb.nodesource.com/setup_20.x — Node.js 20 LTS "Iron" (recommended)
   * https://deb.nodesource.com/setup_21.x — Node.js 21 "Iron" (current)
   


  Please see https://github.com/nodejs/Release for details about which
  version may be appropriate for you.

  The NodeSource Node.js distributions repository contains
  information both about supported versions of Node.js and supported Linux
  distributions. To learn more about usage, see the repository:
   https://github.com/nodesource/distributions

================================================================================
================================================================================

Continuing in 10 seconds ...

2025-06-06 11:28:03 - Installing pre-requisites
Hit:1 http://http.kali.org/kali kali-rolling InRelease
Hit:2 https://repo.protonvpn.com/debian stable InRelease
Reading package lists... Done
W: http://http.kali.org/kali/dists/kali-rolling/InRelease: Key is stored in legacy trusted.gpg keyring (/etc/apt/trusted.gpg), see the DEPRECATION section in apt-key(8) for details.
N: Repository 'Kali Linux' changed its 'non-free component' value from 'non-free' to 'non-free non-free-firmware'
N: More information about this can be found online at: https://www.kali.org/blog/non-free-firmware-transition/
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
curl is already the newest version (8.13.0-5).
curl set to manually installed.
gnupg is already the newest version (2.4.7-19).
gnupg set to manually installed.
The following packages were automatically installed and are no longer required:
  libpython3.12-dev python3.12 python3.12-dev python3.12-minimal python3.12-venv
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  apt apt-utils libapt-pkg7.0 sqv
The following NEW packages will be installed:
  apt-transport-https libapt-pkg7.0 sqv
The following packages will be upgraded:
  apt apt-utils ca-certificates
3 upgraded, 3 newly installed, 0 to remove and 1693 not upgraded.
Need to get 3,763 kB of archives.
After this operation, 5,941 kB of additional disk space will be used.
Get:1 http://kali.download/kali kali-rolling/main amd64 sqv amd64 1.3.0-2 [661 kB]
Get:2 http://http.kali.org/kali kali-rolling/main amd64 libapt-pkg7.0 amd64 3.0.1+kali1 [1,113 kB]
Get:3 http://http.kali.org/kali kali-rolling/main amd64 apt amd64 3.0.1+kali1 [1,453 kB]
Get:5 http://kali.download/kali kali-rolling/main amd64 ca-certificates all 20250419 [162 kB]
Get:6 http://http.kali.org/kali kali-rolling/main amd64 apt-transport-https all 3.0.1+kali1 [38.8 kB]
Get:4 http://http.kali.org/kali kali-rolling/main amd64 apt-utils amd64 3.0.1+kali1 [336 kB]
Fetched 3,763 kB in 1s (2,875 kB/s)
Preconfiguring packages ...
Selecting previously unselected package sqv.
(Reading database ... 434633 files and directories currently installed.)
Preparing to unpack .../archives/sqv_1.3.0-2_amd64.deb ...
Unpacking sqv (1.3.0-2) ...
Setting up sqv (1.3.0-2) ...
Selecting previously unselected package libapt-pkg7.0:amd64.
(Reading database ... 434643 files and directories currently installed.)
Preparing to unpack .../libapt-pkg7.0_3.0.1+kali1_amd64.deb ...
Unpacking libapt-pkg7.0:amd64 (3.0.1+kali1) ...
Setting up libapt-pkg7.0:amd64 (3.0.1+kali1) ...
(Reading database ... 434692 files and directories currently installed.)
Preparing to unpack .../apt_3.0.1+kali1_amd64.deb ...
Unpacking apt (3.0.1+kali1) over (2.9.10+kali1) ...
Setting up apt (3.0.1+kali1) ...
(Reading database ... 434687 files and directories currently installed.)
Preparing to unpack .../apt-utils_3.0.1+kali1_amd64.deb ...
Unpacking apt-utils (3.0.1+kali1) over (2.9.10+kali1) ...
Preparing to unpack .../ca-certificates_20250419_all.deb ...
Unpacking ca-certificates (20250419) over (20240203) ...
Selecting previously unselected package apt-transport-https.
Preparing to unpack .../apt-transport-https_3.0.1+kali1_all.deb ...
Unpacking apt-transport-https (3.0.1+kali1) ...
Setting up apt-utils (3.0.1+kali1) ...
Setting up apt-transport-https (3.0.1+kali1) ...
Setting up ca-certificates (20250419) ...
Updating certificates in /etc/ssl/certs...
rehash: warning: skipping ca-certificates.crt, it does not contain exactly one certificate or CRL
9 added, 5 removed; done.
Processing triggers for libc-bin (2.40-3) ...
Processing triggers for man-db (2.13.0-1) ...
Processing triggers for kali-menu (2024.4.0) ...
Processing triggers for ca-certificates (20250419) ...
Updating certificates in /etc/ssl/certs...
0 added, 0 removed; done.
Running hooks in /etc/ca-certificates/update.d...
done.
Processing triggers for ca-certificates-java (20240118) ...
done.
gpg: WARNING: unsafe ownership on homedir '/home/kali/.gnupg'
Get:1 https://deb.nodesource.com/node_16.x nodistro InRelease [12.1 kB]
Hit:2 http://http.kali.org/kali kali-rolling InRelease                          
Err:2 http://http.kali.org/kali kali-rolling InRelease
  Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
Hit:3 https://repo.protonvpn.com/debian stable InRelease
Get:4 https://deb.nodesource.com/node_16.x nodistro/main amd64 Packages [7,462 B]
Get:5 https://deb.nodesource.com/node_16.x nodistro/main amd64 Contents (deb) [19.5 kB]
Fetched 39.1 kB in 2s (24.4 kB/s)        
Reading package lists... Done
W: https://deb.nodesource.com/node_16.x/dists/nodistro/InRelease: Policy will reject signature within a year, see --audit for details
W: An error occurred during the signature verification. The repository is not updated and the previous index files will be used. OpenPGP signature verification failed: http://http.kali.org/kali kali-rolling InRelease: Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
W: Failed to fetch http://http.kali.org/kali/dists/kali-rolling/InRelease  Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
W: Some index files failed to download. They have been ignored, or old ones used instead.
2025-06-06 11:28:22 - Repository configured successfully. To install Node.js, run: apt-get install nodejs -y
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo apt-get install -y nodejs                   
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
nodejs is already the newest version (20.19.2+dfsg-1).
The following packages were automatically installed and are no longer required:
  libpython3.12-dev python3.12 python3.12-dev python3.12-minimal python3.12-venv
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 1693 not upgraded.
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo npm install -g @proton/cli                  
npm WARN deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated node-domexception@1.0.0: Use your platform's native DOMException instead
npm WARN deprecated ethereumjs-abi@0.6.8: This library has been deprecated and usage is discouraged.
npm WARN deprecated eth-sig-util@3.0.1: Deprecated in favor of '@metamask/eth-sig-util'
npm WARN deprecated @oclif/screen@3.0.8: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/errors@1.3.6: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/help@1.0.15: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/config@1.18.16: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/parser@3.8.17: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
npm WARN deprecated lodash.isequal@4.5.0: This package is deprecated. Use require('node:util').isDeepStrictEqual instead.
npm WARN deprecated @oclif/command@1.8.36: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/config@1.18.2: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/errors@1.3.5: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/config@1.18.17: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm ERR! code EEXIST
npm ERR! path /usr/local/bin/proton
npm ERR! EEXIST: file already exists
npm ERR! File exists: /usr/local/bin/proton
npm ERR! Remove the existing file and try again, or run npm
npm ERR! with --force to overwrite files recklessly.

npm ERR! A complete log of this run can be found in:
npm ERR!     /root/.npm/_logs/2025-06-06T15_32_33_132Z-debug-0.log
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo chown -R $USER /usr/local/lib/node_modules
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo chown -R $USER /usr/local/bin             
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ proton --version
node:internal/modules/cjs/loader:1215
  throw err;
  ^

Error: Cannot find module './lib/Runner'
Require stack:
- /usr/local/lib/node_modules/proton-cli/index.js
- /usr/local/lib/node_modules/proton-cli/bin/proton.js
    at Module._resolveFilename (node:internal/modules/cjs/loader:1212:15)
    at Module._load (node:internal/modules/cjs/loader:1043:27)
    at Module.require (node:internal/modules/cjs/loader:1298:19)
    at require (node:internal/modules/helpers:182:18)
    at Object.<anonymous> (/usr/local/lib/node_modules/proton-cli/index.js:2:16)
    at Module._compile (node:internal/modules/cjs/loader:1529:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1613:10)
    at Module.load (node:internal/modules/cjs/loader:1275:32)
    at Module._load (node:internal/modules/cjs/loader:1096:12)
    at Module.require (node:internal/modules/cjs/loader:1298:19) {
  code: 'MODULE_NOT_FOUND',
  requireStack: [
    '/usr/local/lib/node_modules/proton-cli/index.js',
    '/usr/local/lib/node_modules/proton-cli/bin/proton.js'
  ]
}

Node.js v20.19.2
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ proton account:login pearlhunt7895042@gmail.com              
node:internal/modules/cjs/loader:1215
  throw err;
  ^

Error: Cannot find module './lib/Runner'
Require stack:
- /usr/local/lib/node_modules/proton-cli/index.js
- /usr/local/lib/node_modules/proton-cli/bin/proton.js
    at Module._resolveFilename (node:internal/modules/cjs/loader:1212:15)
    at Module._load (node:internal/modules/cjs/loader:1043:27)
    at Module.require (node:internal/modules/cjs/loader:1298:19)
    at require (node:internal/modules/helpers:182:18)
    at Object.<anonymous> (/usr/local/lib/node_modules/proton-cli/index.js:2:16)
    at Module._compile (node:internal/modules/cjs/loader:1529:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1613:10)
    at Module.load (node:internal/modules/cjs/loader:1275:32)
    at Module._load (node:internal/modules/cjs/loader:1096:12)
    at Module.require (node:internal/modules/cjs/loader:1298:19) {
  code: 'MODULE_NOT_FOUND',
  requireStack: [
    '/usr/local/lib/node_modules/proton-cli/index.js',
    '/usr/local/lib/node_modules/proton-cli/bin/proton.js'
  ]
}

Node.js v20.19.2
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo apt-get install python3-keyring
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
python3-keyring is already the newest version (25.6.0-2).
python3-keyring set to manually installed.
The following packages were automatically installed and are no longer required:
  libpython3.12-dev python3.12 python3.12-dev python3.12-minimal python3.12-venv
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 1693 not upgraded.
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ curl -fsSl https://deb.nodesource.com/setup_16.x | sudo -E bash -

================================================================================
================================================================================

                              DEPRECATION WARNING                            

     Node.js 16.x is no longer actively supported!

  You will not receive security or critical stability updates for this version.

  You should migrate to a supported version of Node.js as soon as possible.
  Use the installation script that corresponds to the version of Node.js you
  wish to install. e.g.
  
   * https://deb.nodesource.com/setup_16.x — Node.js 16 "Gallium" (deprecated)
   * https://deb.nodesource.com/setup_18.x — Node.js 18 "Hydrogen" (Maintenance)
   * https://deb.nodesource.com/setup_19.x — Node.js 19 "Nineteen" (deprecated)
   * https://deb.nodesource.com/setup_20.x — Node.js 20 LTS "Iron" (recommended)
   * https://deb.nodesource.com/setup_21.x — Node.js 21 "Iron" (current)
   


  Please see https://github.com/nodejs/Release for details about which
  version may be appropriate for you.

  The NodeSource Node.js distributions repository contains
  information both about supported versions of Node.js and supported Linux
  distributions. To learn more about usage, see the repository:
   https://github.com/nodesource/distributions

================================================================================
================================================================================

Continuing in 10 seconds ...

2025-06-06 11:42:21 - Installing pre-requisites
Hit:1 https://deb.nodesource.com/node_16.x nodistro InRelease
Hit:2 http://http.kali.org/kali kali-rolling InRelease                
Err:2 http://http.kali.org/kali kali-rolling InRelease                
  Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
Hit:3 https://repo.protonvpn.com/debian stable InRelease
Reading package lists... Done
W: https://deb.nodesource.com/node_16.x/dists/nodistro/InRelease: Policy will reject signature within a year, see --audit for details
W: An error occurred during the signature verification. The repository is not updated and the previous index files will be used. OpenPGP signature verification failed: http://http.kali.org/kali kali-rolling InRelease: Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
W: Failed to fetch http://http.kali.org/kali/dists/kali-rolling/InRelease  Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
W: Some index files failed to download. They have been ignored, or old ones used instead.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
apt-transport-https is already the newest version (3.0.1+kali1).
ca-certificates is already the newest version (20250419).
curl is already the newest version (8.13.0-5).
gnupg is already the newest version (2.4.7-19).
The following packages were automatically installed and are no longer required:
  libpython3.12-dev python3.12 python3.12-dev python3.12-minimal python3.12-venv
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 1693 not upgraded.
gpg: WARNING: unsafe ownership on homedir '/home/kali/.gnupg'
Hit:1 https://repo.protonvpn.com/debian stable InRelease
Hit:2 http://http.kali.org/kali kali-rolling InRelease     
Err:2 http://http.kali.org/kali kali-rolling InRelease     
  Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
Hit:3 https://deb.nodesource.com/node_16.x nodistro InRelease
Reading package lists... Done        
W: An error occurred during the signature verification. The repository is not updated and the previous index files will be used. OpenPGP signature verification failed: http://http.kali.org/kali kali-rolling InRelease: Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
W: https://deb.nodesource.com/node_16.x/dists/nodistro/InRelease: Policy will reject signature within a year, see --audit for details
W: Failed to fetch http://http.kali.org/kali/dists/kali-rolling/InRelease  Sub-process /usr/bin/sqv returned an error code (1), error message is: Missing key 827C8569F2518CC677FECA1AED65462EC8D5E4C5, which is needed to verify signature.
W: Some index files failed to download. They have been ignored, or old ones used instead.
2025-06-06 11:42:26 - Repository configured successfully. To install Node.js, run: apt-get install nodejs -y
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo apt-get install -y nodejs      
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
nodejs is already the newest version (20.19.2+dfsg-1).
The following packages were automatically installed and are no longer required:
  libpython3.12-dev python3.12 python3.12-dev python3.12-minimal python3.12-venv
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 1693 not upgraded.
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ node -v   
v20.19.2
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ npm -v    
9.2.0
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo npm install -g @proton/cli
npm WARN deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
npm WARN deprecated @oclif/screen@3.0.8: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated lodash.isequal@4.5.0: This package is deprecated. Use require('node:util').isDeepStrictEqual instead.
npm WARN deprecated rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated eth-sig-util@3.0.1: Deprecated in favor of '@metamask/eth-sig-util'
npm WARN deprecated @oclif/command@1.8.36: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated ethereumjs-abi@0.6.8: This library has been deprecated and usage is discouraged.
npm WARN deprecated @oclif/help@1.0.15: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/errors@1.3.6: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/errors@1.3.5: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/config@1.18.17: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/config@1.18.2: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/config@1.18.16: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated @oclif/parser@3.8.17: Package no longer supported. Contact Support at https://www.npmjs.com/support for more info.
npm WARN deprecated node-domexception@1.0.0: Use your platform's native DOMException instead
npm ERR! code EEXIST
npm ERR! path /usr/local/bin/proton
npm ERR! EEXIST: file already exists
npm ERR! File exists: /usr/local/bin/proton
npm ERR! Remove the existing file and try again, or run npm
npm ERR! with --force to overwrite files recklessly.

npm ERR! A complete log of this run can be found in:
npm ERR!     /root/.npm/_logs/2025-06-06T15_43_39_100Z-debug-0.log
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ which proton    
/usr/local/bin/proton
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ proton --version                               
node:internal/modules/cjs/loader:1215
  throw err;
  ^

Error: Cannot find module './lib/Runner'
Require stack:
- /usr/local/lib/node_modules/proton-cli/index.js
- /usr/local/lib/node_modules/proton-cli/bin/proton.js
    at Module._resolveFilename (node:internal/modules/cjs/loader:1212:15)
    at Module._load (node:internal/modules/cjs/loader:1043:27)
    at Module.require (node:internal/modules/cjs/loader:1298:19)
    at require (node:internal/modules/helpers:182:18)
    at Object.<anonymous> (/usr/local/lib/node_modules/proton-cli/index.js:2:16)
    at Module._compile (node:internal/modules/cjs/loader:1529:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1613:10)
    at Module.load (node:internal/modules/cjs/loader:1275:32)
    at Module._load (node:internal/modules/cjs/loader:1096:12)
    at Module.require (node:internal/modules/cjs/loader:1298:19) {
  code: 'MODULE_NOT_FOUND',
  requireStack: [
    '/usr/local/lib/node_modules/proton-cli/index.js',
    '/usr/local/lib/node_modules/proton-cli/bin/proton.js'
  ]
}

Node.js v20.19.2
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ proton account:login pearlhunt7895042@gmail.com
node:internal/modules/cjs/loader:1215
  throw err;
  ^

Error: Cannot find module './lib/Runner'
Require stack:
- /usr/local/lib/node_modules/proton-cli/index.js
- /usr/local/lib/node_modules/proton-cli/bin/proton.js
    at Module._resolveFilename (node:internal/modules/cjs/loader:1212:15)
    at Module._load (node:internal/modules/cjs/loader:1043:27)
    at Module.require (node:internal/modules/cjs/loader:1298:19)
    at require (node:internal/modules/helpers:182:18)
    at Object.<anonymous> (/usr/local/lib/node_modules/proton-cli/index.js:2:16)
    at Module._compile (node:internal/modules/cjs/loader:1529:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1613:10)
    at Module.load (node:internal/modules/cjs/loader:1275:32)
    at Module._load (node:internal/modules/cjs/loader:1096:12)
    at Module.require (node:internal/modules/cjs/loader:1298:19) {
  code: 'MODULE_NOT_FOUND',
  requireStack: [
    '/usr/local/lib/node_modules/proton-cli/index.js',
    '/usr/local/lib/node_modules/proton-cli/bin/proton.js'
  ]
}

Node.js v20.19.2
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ curl ifconfig.me                                                 
202.179.75.2                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ curl ipinfo.io/ip
202.179.75.2                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ ip a        
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host noprefixroute 
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    link/ether 00:0c:29:be:2d:f4 brd ff:ff:ff:ff:ff:ff
    inet 192.168.220.129/24 brd 192.168.220.255 scope global dynamic noprefixroute eth0
       valid_lft 1428sec preferred_lft 1428sec
    inet6 fe80::65ca:7482:c78e:c6b9/64 scope link noprefixroute 
       valid_lft forever preferred_lft forever
                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ hostname -I
192.168.220.129 

My IP Address is:

IPv4: ? 202.179.75.2

IPv6: ? Not detected

                                                                                                                    
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo tcpdump -i any port 443   
tcpdump: WARNING: any: That device doesn't support promiscuous mode
(Promiscuous mode not supported on the "any" device)
tcpdump: verbose output suppressed, use -v[v]... for full protocol decode
listening on any, link-type LINUX_SLL2 (Linux cooked v2), snapshot length 262144 bytes
11:54:52.373987 eth0  In  IP 104.18.27.193.https > 192.168.220.129.36125: UDP, length 539
11:54:52.373988 eth0  In  IP 104.18.27.193.https > 192.168.220.129.36125: UDP, length 35
11:54:52.426996 eth0  In  IP 104.18.27.193.https > 192.168.220.129.57855: UDP, length 539
11:54:52.426997 eth0  In  IP 104.18.27.193.https > 192.168.220.129.57855: UDP, length 35
11:54:53.073085 eth0  Out IP 192.168.220.129.43158 > 194.23.211.130.bc.googleusercontent.com.https: Flags [P.], seq 4262580968:4262581007, ack 1660971824, win 65535, length 39
11:54:53.073236 eth0  Out IP 192.168.220.129.51494 > 31.152.160.34.bc.googleusercontent.com.https: Flags [P.], seq 1585542323:1585542362, ack 2067476889, win 65535, length 39
11:54:53.073297 eth0  Out IP 192.168.220.129.52870 > 104.18.43.90.https: Flags [P.], seq 3404121335:3404121374, ack 1810712301, win 65535, length 39
11:54:53.073344 eth0  Out IP 192.168.220.129.43528 > bom12s14-in-f8.1e100.net.https: Flags [P.], seq 1126881237:1126881276, ack 1857050115, win 65535, length 39
11:54:53.073403 eth0  Out IP 192.168.220.129.58958 > 104.22.74.216.https: Flags [P.], seq 3592100702:3592100741, ack 1822051817, win 63955, length 39
11:54:53.073421 eth0  In  IP 194.23.211.130.bc.googleusercontent.com.https > 192.168.220.129.43158: Flags [.], ack 39, win 64240, length 0
11:54:53.073462 eth0  Out IP 192.168.220.129.34750 > 104.18.20.206.https: Flags [P.], seq 430904539:430904578, ack 434848360, win 65535, length 39
11:54:53.073502 eth0  In  IP 31.152.160.34.bc.googleusercontent.com.https > 192.168.220.129.51494: Flags [.], ack 39, win 64240, length 0
11:54:53.073502 eth0  In  IP 104.18.43.90.https > 192.168.220.129.52870: Flags [.], ack 39, win 64240, length 0
11:54:53.073502 eth0  In  IP bom12s14-in-f8.1e100.net.https > 192.168.220.129.43528: Flags [.], ack 39, win 64240, length 0
11:54:53.073502 eth0  In  IP 104.22.74.216.https > 192.168.220.129.58958: Flags [.], ack 39, win 64240, length 0
11:54:53.073703 eth0  In  IP 104.18.20.206.https > 192.168.220.129.34750: Flags [.], ack 39, win 64240, length 0
11:54:53.076504 eth0  In  IP bom12s14-in-f8.1e100.net.https > 192.168.220.129.43528: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:53.076525 eth0  Out IP 192.168.220.129.43528 > bom12s14-in-f8.1e100.net.https: Flags [.], ack 40, win 65535, length 0
11:54:53.076747 eth0  In  IP 31.152.160.34.bc.googleusercontent.com.https > 192.168.220.129.51494: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:53.076767 eth0  Out IP 192.168.220.129.51494 > 31.152.160.34.bc.googleusercontent.com.https: Flags [.], ack 40, win 65535, length 0
11:54:53.077701 eth0  In  IP 194.23.211.130.bc.googleusercontent.com.https > 192.168.220.129.43158: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:53.077701 eth0  In  IP 104.18.43.90.https > 192.168.220.129.52870: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:53.077701 eth0  In  IP 104.18.20.206.https > 192.168.220.129.34750: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:53.077716 eth0  Out IP 192.168.220.129.43158 > 194.23.211.130.bc.googleusercontent.com.https: Flags [.], ack 40, win 65535, length 0
11:54:53.077736 eth0  Out IP 192.168.220.129.52870 > 104.18.43.90.https: Flags [.], ack 40, win 65535, length 0
11:54:53.077750 eth0  Out IP 192.168.220.129.34750 > 104.18.20.206.https: Flags [.], ack 40, win 65535, length 0
11:54:53.088118 eth0  In  IP 104.22.74.216.https > 192.168.220.129.58958: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:53.088146 eth0  Out IP 192.168.220.129.58958 > 104.22.74.216.https: Flags [.], ack 40, win 63916, length 0
11:54:54.423057 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1067
11:54:54.423476 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1357
11:54:54.429505 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 1200
11:54:54.429506 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 1200
11:54:54.429506 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 1200
11:54:54.429831 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 1052
11:54:54.431015 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 54
11:54:54.432740 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 172
11:54:54.432828 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 77
11:54:54.434551 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 96
11:54:54.435062 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.54328: UDP, length 379
11:54:54.435063 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.54328: UDP, length 43
11:54:54.435327 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 44
11:54:54.435795 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 1452
11:54:54.435796 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 107
11:54:54.435796 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 43
11:54:54.435925 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 96
11:54:54.437422 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 43
11:54:54.437502 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 96
11:54:54.438005 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.54328: UDP, length 43
11:54:54.444802 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.59026: UDP, length 43
11:54:54.444937 eth0  Out IP 192.168.220.129.59026 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 96
11:54:54.502648 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1067
11:54:54.513492 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.54328: UDP, length 377
11:54:54.513492 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.54328: UDP, length 43
11:54:54.513853 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 44
11:54:54.519900 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.54328: UDP, length 43
11:54:54.533336 eth0  In  IP 104.18.27.193.https > 192.168.220.129.36125: UDP, length 539
11:54:54.533337 eth0  In  IP 104.18.27.193.https > 192.168.220.129.36125: UDP, length 35
11:54:54.847517 eth0  In  IP 104.18.27.193.https > 192.168.220.129.36640: UDP, length 539
11:54:54.847518 eth0  In  IP 104.18.27.193.https > 192.168.220.129.36640: UDP, length 35
11:54:55.074573 eth0  Out IP 192.168.220.129.38360 > 104.22.11.199.https: Flags [P.], seq 3395277755:3395277794, ack 55656826, win 65535, length 39
11:54:55.074702 eth0  Out IP 192.168.220.129.45654 > server-108-158-46-89.bom78.r.cloudfront.net.https: Flags [P.], seq 1140825764:1140825803, ack 1455470106, win 57654, length 39
11:54:55.074765 eth0  Out IP 192.168.220.129.44262 > server-108-158-61-94.bom78.r.cloudfront.net.https: Flags [P.], seq 1627348286:1627348325, ack 1292214660, win 65535, length 39
11:54:55.074819 eth0  Out IP 192.168.220.129.33316 > 207.65.33.78.https: Flags [P.], seq 2116073825:2116073864, ack 1424235981, win 65535, length 39
11:54:55.074855 eth0  Out IP 192.168.220.129.41584 > bom12s08-in-f3.1e100.net.https: Flags [P.], seq 4126395077:4126395116, ack 439505271, win 65535, length 39
11:54:55.074893 eth0  Out IP 192.168.220.129.47860 > 86.39.117.34.bc.googleusercontent.com.https: Flags [P.], seq 4204263498:4204263537, ack 1017807199, win 65535, length 39
11:54:55.074970 eth0  In  IP 104.22.11.199.https > 192.168.220.129.38360: Flags [.], ack 39, win 64240, length 0
11:54:55.074971 eth0  In  IP server-108-158-46-89.bom78.r.cloudfront.net.https > 192.168.220.129.45654: Flags [.], ack 39, win 64240, length 0
11:54:55.074981 eth0  Out IP 192.168.220.129.44276 > server-108-158-61-94.bom78.r.cloudfront.net.https: Flags [P.], seq 1629486391:1629486430, ack 1531328404, win 65535, length 39
11:54:55.075028 eth0  Out IP 192.168.220.129.47204 > ec2-3-0-107-214.ap-southeast-1.compute.amazonaws.com.https: Flags [P.], seq 19343311:19343350, ack 527665907, win 65535, length 39
11:54:55.075082 eth0  In  IP server-108-158-61-94.bom78.r.cloudfront.net.https > 192.168.220.129.44262: Flags [.], ack 39, win 64240, length 0
11:54:55.075083 eth0  In  IP 207.65.33.78.https > 192.168.220.129.33316: Flags [.], ack 39, win 64240, length 0
11:54:55.075083 eth0  In  IP bom12s08-in-f3.1e100.net.https > 192.168.220.129.41584: Flags [.], ack 39, win 64240, length 0
11:54:55.075083 eth0  In  IP 86.39.117.34.bc.googleusercontent.com.https > 192.168.220.129.47860: Flags [.], ack 39, win 64240, length 0
11:54:55.075083 eth0  In  IP server-108-158-61-94.bom78.r.cloudfront.net.https > 192.168.220.129.44276: Flags [.], ack 39, win 64240, length 0
11:54:55.075366 eth0  In  IP ec2-3-0-107-214.ap-southeast-1.compute.amazonaws.com.https > 192.168.220.129.47204: Flags [.], ack 39, win 64240, length 0
11:54:55.077985 eth0  In  IP bom12s08-in-f3.1e100.net.https > 192.168.220.129.41584: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.078011 eth0  Out IP 192.168.220.129.41584 > bom12s08-in-f3.1e100.net.https: Flags [.], ack 40, win 65535, length 0
11:54:55.078866 eth0  In  IP server-108-158-61-94.bom78.r.cloudfront.net.https > 192.168.220.129.44276: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.078867 eth0  In  IP server-108-158-46-89.bom78.r.cloudfront.net.https > 192.168.220.129.45654: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.078867 eth0  In  IP server-108-158-61-94.bom78.r.cloudfront.net.https > 192.168.220.129.44262: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.078867 eth0  In  IP 104.22.11.199.https > 192.168.220.129.38360: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.078892 eth0  Out IP 192.168.220.129.44276 > server-108-158-61-94.bom78.r.cloudfront.net.https: Flags [.], ack 40, win 65535, length 0
11:54:55.078917 eth0  Out IP 192.168.220.129.38360 > 104.22.11.199.https: Flags [.], ack 40, win 65535, length 0
11:54:55.093758 eth0  In  IP 86.39.117.34.bc.googleusercontent.com.https > 192.168.220.129.47860: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.122571 eth0  Out IP 192.168.220.129.44262 > server-108-158-61-94.bom78.r.cloudfront.net.https: Flags [.], ack 40, win 65535, length 0
11:54:55.122691 eth0  Out IP 192.168.220.129.45654 > server-108-158-46-89.bom78.r.cloudfront.net.https: Flags [.], ack 40, win 57615, length 0
11:54:55.134405 eth0  Out IP 192.168.220.129.47860 > 86.39.117.34.bc.googleusercontent.com.https: Flags [.], ack 40, win 65535, length 0
11:54:55.134535 eth0  In  IP 207.65.33.78.https > 192.168.220.129.33316: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.134571 eth0  Out IP 192.168.220.129.33316 > 207.65.33.78.https: Flags [.], ack 40, win 65535, length 0
11:54:55.145528 eth0  In  IP ec2-3-0-107-214.ap-southeast-1.compute.amazonaws.com.https > 192.168.220.129.47204: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:55.145557 eth0  Out IP 192.168.220.129.47204 > ec2-3-0-107-214.ap-southeast-1.compute.amazonaws.com.https: Flags [.], ack 40, win 65535, length 0
11:54:56.111024 eth0  Out IP 192.168.220.129.35296 > 13.107.246.68.https: Flags [P.], seq 4161798156:4161798195, ack 516612889, win 65535, length 39
11:54:56.111136 eth0  Out IP 192.168.220.129.39992 > ec2-52-18-136-20.eu-west-1.compute.amazonaws.com.https: Flags [P.], seq 1873899217:1873899256, ack 1291357416, win 65535, length 39
11:54:56.111209 eth0  Out IP 192.168.220.129.45162 > server-18-66-41-34.bom78.r.cloudfront.net.https: Flags [P.], seq 2738860707:2738860746, ack 768501050, win 65535, length 39
11:54:56.111282 eth0  Out IP 192.168.220.129.36784 > 239.152.111.34.bc.googleusercontent.com.https: Flags [P.], seq 1509768135:1509768174, ack 1240096885, win 65535, length 39
11:54:56.111379 eth0  In  IP 13.107.246.68.https > 192.168.220.129.35296: Flags [.], ack 39, win 64240, length 0
11:54:56.111380 eth0  In  IP ec2-52-18-136-20.eu-west-1.compute.amazonaws.com.https > 192.168.220.129.39992: Flags [.], ack 39, win 64240, length 0
11:54:56.111455 eth0  In  IP server-18-66-41-34.bom78.r.cloudfront.net.https > 192.168.220.129.45162: Flags [.], ack 39, win 64240, length 0
11:54:56.111455 eth0  In  IP 239.152.111.34.bc.googleusercontent.com.https > 192.168.220.129.36784: Flags [.], ack 39, win 64240, length 0
11:54:56.115750 eth0  In  IP server-18-66-41-34.bom78.r.cloudfront.net.https > 192.168.220.129.45162: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:56.115783 eth0  Out IP 192.168.220.129.45162 > server-18-66-41-34.bom78.r.cloudfront.net.https: Flags [.], ack 40, win 65535, length 0
11:54:56.115857 eth0  In  IP 239.152.111.34.bc.googleusercontent.com.https > 192.168.220.129.36784: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:56.115857 eth0  In  IP 13.107.246.68.https > 192.168.220.129.35296: Flags [P.], seq 1:40, ack 39, win 64240, length 39
11:54:56.158464 eth0  Out IP 192.168.220.129.35296 > 13.107.246.68.https: Flags [.], ack 40, win 65535, length 0
11:54:56.158534 eth0  Out IP 192.168.220.129.36784 > 239.152.111.34.bc.googleusercontent.com.https: Flags [.], ack 40, win 65535, length 0
11:54:56.165937 eth0  Out IP 192.168.220.129.49473 > 104.18.26.193.https: UDP, length 1357
11:54:56.166033 eth0  Out IP 192.168.220.129.49473 > 104.18.26.193.https: UDP, length 448
11:54:56.166486 eth0  Out IP 192.168.220.129.40682 > 104.18.27.193.https: UDP, length 1357
11:54:56.167587 eth0  Out IP 192.168.220.129.37587 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1357
11:54:56.167852 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1357
11:54:56.167884 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1357
11:54:56.167904 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1357
11:54:56.167928 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 1357
11:54:56.167951 eth0  Out IP 192.168.220.129.54328 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 189
11:54:56.173894 eth0  In  IP 104.18.27.193.https > 192.168.220.129.40682: UDP, length 1200
11:54:56.173894 eth0  In  IP 104.18.26.193.https > 192.168.220.129.49473: UDP, length 27
11:54:56.173895 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 1200
11:54:56.174333 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 1200
11:54:56.174333 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 1200
11:54:56.174333 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 1051
11:54:56.174334 eth0  In  IP 104.18.27.193.https > 192.168.220.129.40682: UDP, length 1200
11:54:56.174334 eth0  In  IP 104.18.27.193.https > 192.168.220.129.40682: UDP, length 1200
11:54:56.174334 eth0  In  IP 104.18.27.193.https > 192.168.220.129.40682: UDP, length 502
11:54:56.175278 eth0  Out IP 192.168.220.129.40682 > 104.18.27.193.https: UDP, length 55
11:54:56.176465 eth0  Out IP 192.168.220.129.37587 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 54
11:54:56.178833 eth0  Out IP 192.168.220.129.37587 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 172
11:54:56.178889 eth0  Out IP 192.168.220.129.37587 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 79
11:54:56.180430 eth0  Out IP 192.168.220.129.37587 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 96
11:54:56.182927 eth0  Out IP 192.168.220.129.40682 > 104.18.27.193.https: UDP, length 149
11:54:56.182967 eth0  Out IP 192.168.220.129.40682 > 104.18.27.193.https: UDP, length 79
11:54:56.183010 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 1452
11:54:56.183022 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 107
11:54:56.183022 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 43
11:54:56.183022 eth0  In  IP server-18-172-78-31.bom78.r.cloudfront.net.https > 192.168.220.129.37587: UDP, length 43
11:54:56.183096 eth0  Out IP 192.168.220.129.37587 > server-18-172-78-31.bom78.r.cloudfront.net.https: UDP, length 96

      
tested internet speed

disconnected vpn
my ip address
IPv4: ? 202.179.75.2

IPv6: ? Not detected	
 
tested internet speed test again


🔐 VPN Encryption and Privacy Features
✅ 1. Encryption
Encryption is the core technology behind VPN privacy.

🔹 Common VPN Encryption Standards:
Encryption	Description	Strength
AES-256	Advanced Encryption Standard with 256-bit key	Military-grade
ChaCha20	Lightweight, faster on mobile	Strong & efficient
RSA-2048/4096	Used for handshake and key exchange	Very secure
Perfect Forward Secrecy (PFS)	Ensures new encryption keys for each session	Protects past sessions if key is compromised

✅ 2. VPN Protocols
These define how your data is transmitted and encrypted:

Protocol	Description	Best Use
OpenVPN	Open-source, secure, highly configurable	General secure browsing
WireGuard	Modern, faster, lightweight	Speed-focused privacy
IKEv2/IPSec	Good on mobile, reconnects quickly	Mobile & roaming
L2TP/IPSec	Older, secure but slower	Basic compatibility

✅ 3. Privacy Features
Feature	How It Helps You
No-logs Policy	VPN doesn't store your browsing activity
Kill Switch	Cuts your internet if VPN drops to prevent IP/DNS leaks
DNS Leak Protection	Ensures DNS requests go through the VPN, not your ISP
Split Tunneling	Lets you route only specific apps or websites through VPN
Obfuscation/Stealth Mode	Hides VPN traffic as regular traffic to bypass censorship
Multihop (Double VPN)	Routes your traffic through two VPN servers for extra privacy

🧠 How Encryption Works in a VPN (Simplified)
You connect to a VPN server (e.g., in Switzerland).

Your device encrypts data using AES-256 or ChaCha20.

The VPN server decrypts it, sends it to the internet.

Responses from websites are encrypted again back to your device.

Your ISP or any third party only sees encrypted traffic—not your activity or destination.

⚠️ Limitations to Know
Limitation	Description
VPN Provider Trust	You’re trusting the VPN to enforce its privacy claims—choose a reputable one.
No Protection from Malware	A VPN doesn’t block viruses or phishing. Use antivirus and good practices.
Not Anonymity Tool	VPN hides your IP but doesn’t make you fully anonymous like Tor.
Performance Drops	Encryption can reduce speed slightly, especially with long-distance servers.

🛡️ Recommended VPNs with Strong Privacy
ProtonVPN – Open-source, based in Switzerland, no logs, supports Tor

Mullvad – Privacy-focused, anonymous signup, strong transparency

NordVPN – Strong security, audited no-logs policy, good speeds



Here’s a concise summary of the benefits and limitations of VPNs:

✅ Benefits of VPNs
Privacy Protection
Encrypts your internet traffic, hiding activity from ISPs, hackers, and surveillance.

Security on Public Wi-Fi
Prevents data theft on unsecured networks (e.g., coffee shops, airports).

Bypass Geo-restrictions
Access region-locked content (e.g., streaming services, websites).

Anonymity
Masks your IP address, making it harder to trace your online activity.

Remote Access
Allows secure connection to a workplace or home network from remote locations.

Avoid Censorship
Helps bypass government or institutional internet blocks (e.g., in restrictive countries).

⚠️ Limitations of VPNs
Reduced Speed
Encryption and routing through remote servers can slow down your connection.

No Full Anonymity
VPNs don’t prevent tracking through cookies, fingerprinting, or if you log in to services.

Trust in VPN Provider
Some VPNs may log data or be vulnerable themselves. Not all are privacy-focused.

Blocked by Some Services
Some websites and apps detect and block VPN traffic (e.g., Netflix, banks).

Cost
Reliable VPNs usually require a paid subscription; free ones may have limits or privacy concerns.

Legality and Policy Risks
VPN usage is restricted or illegal in some countries (e.g., China, Iran, UAE).
