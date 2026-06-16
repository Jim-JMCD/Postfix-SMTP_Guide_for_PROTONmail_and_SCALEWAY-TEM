## A Guide for integrating Postfix with Proton Mail & Scaleway TEM SMTP servcies. 
### Proton STMP is an integrated mail relay add-on to a regular mail account, best for low volume mailing.
### Scaleway transactional SMTP mail service is designed for low and high volume mailing.         

This guide describes how integrate Linux postfix to work with Proton Mail and Scaleway Transactional Email (TEM) secure SMTP services. Postfix when configured to work with a SMTP relay provides system and application administrators to use native and application mail tools to send reports, alerts and other information to external email addresses. The SMTP services of Proton and Scaleway are different in configuration requirements because they are designed for different workloads.    

The guide is for separate installations, it does not cover configuring postfix to use Proton and Scaleway SMTP in the same computer.   
 
#### Guide coverage
* Postfix Installation and configuration with SASL/TLS security.
* Setting default email addresses with __*sender_canonical*__. 
* Enabling preconfigured sender email addresses for Proton SMTP with __*sender_relay*__.
* Configuring cron and rsyslog ommail to send external mail.
* Testing and some troubleshooting.

This guide could be used for other Postfix SMTP mail installations. 
