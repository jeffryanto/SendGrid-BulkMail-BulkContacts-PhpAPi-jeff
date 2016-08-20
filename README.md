SendGrid Bulk Contacts List - PHP
======================

This git repository helps you to send emails quickly and easily through SendGrid using PHP.

Create an SendGrid account at http://sendgrid.com/pricing.html

Clone SendGrid application on your local machine
<pre>
    git clone https://github.com/sendgrid/sendgrid-php-sample-app
</pre>

###Configuration###

Configure `index.php` file with your information:

Update the *&lt;sendgrid_username&gt;* and *&lt;sendgrid_password&gt;* with your SendGrid credentials.
```php
    $sendgrid_username = '<sendgrid_username>';
    $sendgrid_password = '<sendgrid_password>';
```
Update the *&lt;from_address&gt;* with your email address
```php
    $from_email = "<from_address>";
```

Adding Bulk Contacts lists
```php
       $emails = array(
       'test@test.com','test12@test.com','testing@test.com','test23@test.com'
    );
    
```
You can add around 1000 to 2000 mails id's in one set in this array . Emails must be added in ( single quotes comma seperated values )

Adding an Attachment 
```php
      $mail->
      addAttachment("/path/to/attachment/test.jpg");
```
Adding Cc
```php
      $mail
      ->addCc("nptelpsrr@psrr.edu.in");
```
Upload your application to your server




