# Практическое занятие №1. Введение, основы работы в командной строке

## Задача 1

⁓# cut -d: -f1 /etc/passwd | sort

![image](https://github.com/user-attachments/assets/f7e9f15c-b56e-4e7a-a525-816861fe6071)

## Задача 2

~# cat /etc/protocols | sort -k2,2nr | head -n 5 | awk '{print $2, $1}'

![image](https://github.com/user-attachments/assets/bab7397e-2f7c-45b2-afbd-3e86add9e6cc)

## Задача 3

#!/bin/bash

text=$*
length=${#text}

for i in $(seq 1 $((length + 2))); do
    line+="-"
done

echo "+${line}+"
echo "| ${text} |"
echo "+${line}+"


