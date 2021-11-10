http://sandbox.onlinephpfunctions.com/code/a1291493874151f964572a72ad57cbea14055c7d


<?php
        //Enter your code here, enjoy!

$products = [
    [
        "name" => "X-Box One",
        "price" => 450000.00,
        "amount" => 15
    ],
    [
        "name" => "IPhone X",
        "price" => 560000.00,
        "amount" => 6
    ],


];

function my_function(array $products): array
{
    global $products;
    foreach ($products as $key => $product) {
        $products[$key]['shipping_cost '] = $product['price'] * 2 / 100;
    }
    return $products;
}
my_function($products);

print_r($products);

