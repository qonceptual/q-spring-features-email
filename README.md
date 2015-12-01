# Introduction
A Spring based @Service to send emails via Amazon's Simple Email Service

## Installation

Add the following dependency to your Maven/Ivy Project:

`    
<dependency>
    <groupId>com.qonceptual</groupId>
    <artifactId>q-spring-features-email</artifactId>
    <version>1.0.0</version>
</dependency>
`

Add `com.qonceptual.*` in as part of you component scan.
 
For ex: `@ComponentScan(basePackages = {"com.qonceptual.*"})`

Add the following configurations to your Spring or Spring Boot property files:

`qonceptual.spring.email.ses.accessKey = AWSACCESSKEY
 qonceptual.spring.email.ses.secretKey = AWSSECRETKEY`
  
Inject the SimpleEmailService via the EmailService Interface to the name of "simpleEmailService".

`@Autowired
 private EmailService simpleEmailService;`
 
That's it!