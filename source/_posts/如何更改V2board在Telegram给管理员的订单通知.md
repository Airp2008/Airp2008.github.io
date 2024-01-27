本作以V2board 1.7.4为示例

需要修改的文件
`app\Http\Controllers\Guest\PaymentController.php`

在29行至48行中为本次修改的部分

推荐模板:
`
$message = sprintf(
"订单号: %s\n收款: %s元",
$order->trade_no,
$order->total_amount / 100,
);`