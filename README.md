# DOCUMENTATION
Official QIWI developer page: https://developer.qiwi.com/ru/qiwi-wallet-personal/#intro <br>
Source: https://github.com/Shnapik/Qiwi-Api-Class-PHP/blob/master/src/Qiwi.php <br>
Official QIWI API page (without send...() functions): https://github.com/QIWI-API/bill-payments-php-sdk <br>

**Connection:**<br>
``` require_once 'path to file Qiwi.php';```
```
$qiwiData = [
    'phone' => 'qiwi phone number without +',
    'token' => 'qiwi api token'
];
```
```$qiwi = new Qiwi($qiwiData['phone'], $qiwiData['token'], false);```

**Basic function:**<br>
```
$walletBalance = $qiwi->getBalance();
var_dump($walletBalance);
```

# FUNCTIONS
<b>getProfile()</b> - Information about account <br>
<b>getIdentification()</b> - Information about account identification<br>
<b>getLimits()</b> - Active limits, that account has<br>
<b>getRestrictions()</b> - Shows if there are any restrictions and information about them<br>
<b>getPaymentsHistory()</b> - Payment history<br>
<b>getPaymentsStats()</b> - Payment statistics between chosen dates<br>
<b>getPaymentInfo()</b> - Information about current payment<br>
<b>getCheque()</b> - Cheque of current payment JPG/PDF<br>
<b>getBalance()</b> - Current balance<br>
<b>getTax()</b> - Tax, that you will pay by sending moneyy to a current account<br>
<b>getBills()</b> - Check your bills<br>
<b>getMyNickName()</b> - Shows account nickname<br>
<b>sendIdentification()</b> - Sends identification to QIWI (didnt check it though)<br>
<b>sendMoneyToQiwi()</b> - Send money without confirmation to someone<br>
<b>sendConverted()</b> - Transferring funds to a foreign currency account QIWI Wallet with conversion from your ruble account.<br>
<b>sendMoneyToOther()</b> - Send money by card num.<br>
<b>sendBillPayment()</b> - Pay summ by bill number<br>
