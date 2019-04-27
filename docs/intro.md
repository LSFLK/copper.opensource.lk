# Copper Mail solution

</br>
Copper email solution can be used by any organization and can be monitored and controled from a central access point. It consists of 2 main parts

1. [Copper-server](https://github.com/LSFLK/Copper/tree/master/copper-server)
2. [Copper-hub](https://github.com/LSFLK/Copper/tree/master/copper-hub)

</br>
## Copper-server

### Architecture

![Octocat](images/copperBase_mailServerArchitecture.png)


#### Copper-server main components.

- [Postfix](http://www.postfix.org/) : A modular mail transfer agent (MTA)
- [Dovecot](https://www.dovecot.org/) : Secure open-source IMAP and POP3 server (MDA)
- [ClamAV](https://www.clamav.net/) : Antivirus software
- [Rspamd](https://rspamd.com/) : Spam filter
- [Group-Office](https://www.group-office.com/) : Web client to access mail for users
- [OpenLDAP](https://www.openldap.org/) : Directory service which authenticate users

</br>
## Contributors are wellcome

Due to this is an opensource project, contributors are welcome.
Copper-server readme file describe how to use this solution in development environments.
So any one whom, willing to contribute are wellcome and coppermail team is ready to support.

</br>
## Copper Versioning 

version number **MAJOR.MINOR.PATCH**, increment the:

- **MAJOR** version with incompatible API changes,
- **MINOR** version with functionality in a backwards-compatible manner, and
- **PATCH** version with backwards-compatible bug fixes.

Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

Additional labels  **alpha** | **beta** | **RC** 
- **alpha** = A feature complete version 
- **beta**  = A tested and improved version without having any level one issues. 
- **RC**  = Release Candidate, version of a program that is ready for  a complete release. 

</br>
## Further readings

  1. [Ready to deploy email solution](https://docs.google.com/document/d/103ApdgqkJtV1fE3tVQKIwE-ldxtfBPKsAVjk8GFpLb8/edit#heading=h.tca36t2d12pa)

</br>
## Instruction for deployment (summary)


#### Create environment

1. Clone the repository [Copper](https://github.com/LSFLK/Copper.git) and refer [this](https://github.com/LSFLK/Copper/blob/master/copper-server/README.md) document for install Copper.

```
$ git clone https://github.com/LSFLK/Copper.git
```


#### Stay in touch with us.

- [mail group](https://groups.google.com/forum/#!forum/lsf-email-solution) 
- [![Gitter](https://img.shields.io/badge/chat-on%20gitter-blue.svg)](https://gitter.im/copper-mail)