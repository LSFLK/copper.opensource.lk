

## Features to be enabled in future

<p align="justify">
Copper has planned many new features to be implemented in copper solution. Those planned features can be summarized hear for further validation and contribution . Git issues opened for these feature are also mentioned hear.
</p>


## 1.  End to end encription

(System related - Enable end-to-end encryption of mail with centralized key management #208)

It is expected enable end to end encription for copper email solution. Thats mean sender sending encripted emails and receivers only can receive the email. This is the PGP (Pritty Good Privacy) protocol does. It will be required a centralized key management system too. So copper is expecting to implement this type of machanism in future.

## 2.  Backups

(Backups - Enable mail storage replication #207)

(Mail archiving, backup and recovery #61)

Backup is very important and critical matter in any email system. In copper we have found 4 items to backup for any client.
*   User base (as export.ldif)
*   Mail dir (Each client's mail directory)
*   Database dump (Group office store data in the database)
*   Configuration (kubernetes secret file which is created in the deployment)

So It is planned to backup those items in a cloud volume and these backup features to be implemented in future.

## 3.  Updates Handling

(update handling : generic agent model #62)

(Copper Hub - Evaluate backup & recovery solutions based on K8s infrastructure #204)

Once a update happens in a docker image those changes should be updated in production systems. It was planned to do using kubernetes update handling mechanisms. To enable it clients may have to activate CI/CD pipe lines in there productions with k8s.

## 4.  Email Rules

(Rules creation for email #224)

(option for Remove email rule(s) #135)

(Update existing email rules #134)

(Apply a rule to future messages #133)

(Apply a rule to future messages #133)

(Create and save rule for emails #132)

Email Rules are very important part for searching vise. But the currently there is a issue in our gropuoffice installation that Email Rules section is disabled. So we are unable work with email rules.
But it is required to deep study on groupoffice codebase and check for a solution.


## 5.  Test Automation

(Test Automation using selenium #192)

After each feature enabling we have to go through lot of testings manually before it is released.
But it is possible to automate all test cases using a tool like selenium. So it is expected to automate all prerelease testings using selenium.

## 6.  TLS with GroupOffice and LDAP server

(TLS activation between LDAP server and Group Office #195)

It was not possible to activate TLS for communication between LDAP server and the GroupOffice with the locally generated key files using ssl. Error was invalied certificate files. So this bug to be investigated and findout a solution.

## 7.   Copper Hub

(Copper Hub - Evaluate backup & recovery solutions based on K8s infrastructure #204)

Copper hub is a cerntralized monitoring system for copper solution deployments. Each users can deploy there own copper solutions. But for monitoring, update handling and services will be provided through copper hub.
So there should be a secrured generic copper hub implemented in some whare in the cloud. Currently we have a initial version of copper hub using prometheus stack. It has to be enhanced to do above functions too. This copper hub repostitoy can be found from bellow git url.

https://github.com/LSFLK/Copper-hub


At the completion of the copper email solution it will have above mentioned features also.


