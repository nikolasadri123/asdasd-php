Skip to content
 
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 @nikolasadri123 Sign out
0
0 1 rehanchrl/vendingMachine
 Code  Issues 0  Pull requests 0  Projects 0  Wiki  Insights
vendingMachine/vending.php
@rehanchrl rehanchrl final release
12126f1  on Apr 8, 2018
56 lines (46 sloc)  839 Bytes
    
<?php
$coin = array ( 
    50000 => '50 ribu', 
    20000 => '20 ribu', 
    10000 => '10 ribu', 
    5000 => '5 ribu', 
    2000 => '2 ribu', 
    1000 => '1 ribu', 
    500 => '5 ratus' );
// uang yang diberikan
$base = 50000;
// harga
$cost = 27000;
// total
$total = $base - $cost;
$out = array ();
$num = 0;
if ( $total > 0 )
{
	foreach ( $coin AS $cn => $cv )
	{
		if ( $total >= $cn )
		{
			while ( $total >= $cn )
			{
				$out[$num] += 1;
				$total -= $cn;
			}
            if ( $out[$num] > 1 )
			{
				$add = ( is_array ( $cv ) ? $cv[1] : $cv . 's' );
			}
			else
			{
				$add = ( is_array ( $cv ) ? $cv[0] : $cv );
            }
            
			$out[$num] = $out[$num] . ' lembar ' . $add;
			$num++;
		}
	}
	echo "kembalian = <br />" . implode ( "<br />dan<br />", $out );
		
}
else
{
	echo 'no change to give';
}
© 2019 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About
