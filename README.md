Scenario There is a customer who came to you with a problem to have a custom linux
command for his operations. Your task is to understand the problem and create a linux
command via bash script as per the instructions.
Command name - internsctl
Command version - v0.1.0

Section A
1. I want a manual page of command so that I can see the full documentation of the command.
--- I do not use the man command and instead opt for the cat command when performing operations on Git Bash.

as output we get the doc and usage guidelines. Similarly if I execute man internsctl I want
to see the manual of my command.

cat internsctl
---
<img width="960" alt="2024-01-10 (4)" src="https://github.com/Vanika-08/xenonstack_task1/assets/141993407/6e1ed49b-d25e-46c5-a98a-68328367679d">
<img width="960" alt="2024-01-10 (3)" src="https://github.com/Vanika-08/xenonstack_task1/assets/141993407/34205d46-b4d8-4c01-bfd5-b21b78b91b28">


3.Each linux command has an option --help which helps the end user to understand the use cases via examples. Similarly if I execute internsctl --help it should provide me the
necessary help
internsctl --help
---

<img width="960" alt="2024-01-10 (5)" src="https://github.com/Vanika-08/xenonstack_task1/assets/141993407/182a365c-7a1a-444f-a666-c4d9057a2c2f">

4.I want to see version of my command by executing
internsctl --version
---
<img width="960" alt="2024-01-10 (6)" src="https://github.com/Vanika-08/xenonstack_task1/assets/141993407/4c5da34c-1c96-4f96-9a85-250dddbce00b">




Section B
---
Part1 | Level Easy

I want to get cpu information of my server through the following command:
$ internsctl cpu getinfo
---
<img width="960" alt="2024-01-10 (7)" src="https://github.com/Vanika-08/xenonstack_task1/assets/141993407/9ae3cb5d-6e17-4d41-bee0-88b1fd76469e">

I want to get memory information of my server through the following command:
$ internsctl memory getinfo
---
<img width="960" alt="2024-01-10 (8)" src="https://github.com/Vanika-08/xenonstack_task1/assets/141993407/1aac94a3-9e83-4a24-b005-6ffd4412024c">


Part2 | Level Intermediate
I want to create a new user on my server through the following command:
$ internsctl user create <username>
---
![image](https://github.com/Vanika-08/xenonstack_task1/assets/141993407/03133809-6b04-4aaf-b65c-28934beee0a9)

I want to list all the regular users present on my server through the following command:
$ internsctl user list
---
![image](https://github.com/Vanika-08/xenonstack_task1/assets/141993407/28ad8d2f-6ca0-4107-b8e4-cd9009574006)

If want to list all the users with sudo permissions on my server through the following command:
$ internsctl user list --sudo-only
![image](https://github.com/Vanika-08/xenonstack_task1/assets/141993407/25ddf61b-7b88-483a-8597-132797c14e39)

Part3 | Advanced Level
By executing below command I want to get some information about a file
$ internsctl file getinfo <file-name>
---
<img width="960" alt="2024-01-10 (9)" src="https://github.com/Vanika-08/xenonstack_task1/assets/141993407/b80b9096-0384-486d-b946-037a12903790">

If I want to obtain the size of the specified file only, I should be able to use the following command:
$ internsctl file getinfo hello.txt --size
---
![image](https://github.com/Vanika-08/xenonstack_task1/assets/141993407/e517360e-1d5e-4acf-97be-39b2bf145d00)

If I want to obtain the permissions of the specified file only, I should be able to use the following
command:
$ internsctl file getinfo hello.txt --permissions
---

![image](https://github.com/Vanika-08/xenonstack_task1/assets/141993407/64640013-2d63-4144-8533-1526cecdc305)

If I want to obtain the owner of the specified file only, I should be able to use the following
command:
$ internsctl file getinfo hello.txt --owner
---

![image](https://github.com/Vanika-08/xenonstack_task1/assets/141993407/cb93bda3-f7a1-44e5-b56d-a4d5bba6485d)


If I want to obtain the last modified time of the specified file only, I should be able to use the
following command:
$ internsctl file getinfo hello.txt --last-modified
---

![image](https://github.com/Vanika-08/xenonstack_task1/assets/141993407/4bbce09a-c0be-4d64-a997-6f3defb7f315)



