# SMS Length Calculator
PHP-based SMS length calculator. Checks if a message can be sent as GSM 7bit charset or if Unicode charset must be used. 

Based on [messente/sms-length-calculator](https://github.com/messente/sms-length-calculator/)
Now Composer-friendly.

Checks if a message can be sent as GSM 7bit charset or if Unicode charset must be used.

## How Install

Just run the following command in your Composer PHP project: 

```
composer require joseorono/sms-length-calculator-composer
```


Composer Package:
https://packagist.org/packages/joseorono/sms-length-calculator-composer

## Usage example

```PHP
$SmsCalc = new SmsLengthCalculator();
$text = "The morpheme can be reduplicated to emphasize the meaning of the word";
$sms_parts = $SmsCalc->getPartCount($text);
echo "Message with text [".$text."] is sent as [".$sms_parts." SMS]\n";
// Output: Message with text [The morpheme can be reduplicated to emphasize the meaning of the word] is sent as [1 SMS]
```

