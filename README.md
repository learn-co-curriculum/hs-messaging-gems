## Messaging APIs with Gems

We're going to look at two messaging APIs that you may want to use in your final projects.

###Twilio and Mailgun

There are two really great web applications that can handle messaging for us. [Twilio](https://www.twilio.com/) is a service used to send text messages from another application. [Mailgun](http://www.mailgun.com/) is a service designed to send emails from a web application. 

Depending on the functionality you would like for your final project, you can use either Twilio or Mailgun.


###Twilio

First things first, you need to have a Twilio account. Because Twilio requires a credit card authorization, please use Flatiron School's account.

We will use the Twilio gem to send texts, [here](https://github.com/twilio/twilio-ruby).

First, you need to install the twilio-ruby gem on your computer. In terminal, from any directory, enter `gem install twilio-ruby`

Next, you will need to follow the instructions found in the README.md file of the gem. You'll want to scroll down till you see the words `Getting Started With REST`.

The only two headers we care about are the instructions under `Setup Work` and `Send an SMS`. We are literally going to copy and paste the code provided into the ruby file in the directory of our final project.

There are a few places that we'll need to fill in with our own data:
auth_token you are going to want to replace with `ACe330ba04d082392df4cb3511dcb72cec` account_sid you'll want to replace with `2008ea097713e401a16c54029058da82` and finally, the from phone number you'll want to replace with `+181526420231`.

You are also going to want to change the body of the text and the number you want to send the text to, but that's up to you!

In order to actually execute this code, you'll just want to run the ruby file. In terminal in the directory of your final project, you'll want to enter `ruby filename.rb`

##Mailgun

To use Mailgun, you will need to create an account from [Mailgun](http://www.mailgun.com/). It's completely free. 

You also need to install the ruby gem on your computer by running in terminal from any directory `gem install mailgun`.

Once you have your account created, you'll want to follow the [README.md for the gem](https://github.com/mailgun/mailgun-ruby). Look for the header `Usage`. The only two sections we need to worry about are `Configuration` and `Sending Email`. You'll want to copy and paste the code in those sections into the ruby file you created in the directory of your final project.

You are going to want to replace the values of  `config.api-key`, `config.domain`, and `:from` with information from your Mailgun account. Your Mailgun domain is going to start with the word `sandbox` and your api-key will start with the word `key`. You should be able to find all of that information on the homepage of the Mailgun site in the logged in state. You will also want to change the subject, body, and receiver of the email, but that's up you! The from email is going to be `postmaster@whatever_your_domain_is`. Obviously subsitute the `whatever_your_domain_is` for that value.

Don't worry about any other instructions that Mailgun tries to provide you. We are using the gem instead of those steps. That's why the gem is there :)

In order to actually execute this code, you'll just want to run the ruby file. In terminal in the directory of your final project, you'll want to enter `ruby filename.rb`

