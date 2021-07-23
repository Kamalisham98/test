# Task 4

#### 1. Make the code below cleaner and readable

```php
public function getPrice() {
        if ($customer->debt > 10000000){
            return error('this customer cannot make a purchase due to his debt over limit');
        }
        if($customer->status != 'active'){
                return error('this customer is not active')
        }

        if($customer->group == 'distributor'){
            return Price::get('distributor');
        }

        if($customer->group == 'general'){
            return Price::get('general');
        }
}
```

#### 2. After change the code, make a pull request
