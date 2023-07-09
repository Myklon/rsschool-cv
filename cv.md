# Illarionov Nikita

## Contacts

* E-mail - <livroklon@gmail.com>
* Telegram - [@Myklon](https://t.me/Myklon);
* GitHub - [Myklon](https://github.com/Myklon);

## About me

I am 23 years old. A novice backend developer who wants to improve his knowledge of frontend

## Skills

* PHP
* MySQL
* Yii2
* Laravel
* Git
* HTML, CSS
* JavaScript (Basic)

## Code
>
> Problem: You are given a 0-indexed integer array tasks, where tasks[i] represents the difficulty level of a task. In each round, you can complete either 2 or 3 tasks of the same difficulty level.
Return the minimum rounds required to complete all the tasks, or -1 if it is not possible to complete all the tasks.

```php

class Solution {

    /**
     * @param Integer[] $tasks
     * @return Integer
     */
     
    function minimumRounds($tasks) {
        $hashArray = [];
        $steps = 0;
        
        foreach ($tasks as $value)
            array_key_exists($value, $hashArray) ? $hashArray[$value]++ : $hashArray[$value] = 1;
        
        if (in_array(1,$hashArray)) return -1;

        foreach ($hashArray as $key => $value)
        {
            $value % 3 == 0 ? $steps += $value / 3 : $steps += (int)($value / 3) + 1;
        }
        
        return $steps;
    }
}
```

## Graduation

*In progress*;

## Languages

* Russian - Native
* English - Intermediate
