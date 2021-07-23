# Task 2

#### 1. Make the code below cleaner, better and reusable

```php
# Add leading 0 number
# ex: 5 => 0005
function convertNumber($number) {
    $number = $number + "";
    let lenghtArr = $number.length;
    for (let i = 1; i <= (4 - lenghtArr); i++) {
        $number = "0" + $number;
  }

  return $number;
}

convertNumber(5);
```

#### 2. After change the code, make a pull request