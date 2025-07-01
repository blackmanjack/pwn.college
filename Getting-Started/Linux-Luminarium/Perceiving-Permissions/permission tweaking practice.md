## Permission Tweaking Practice

You think you can chmod? Let's practice!

This challenge will ask you to change the permissions of the /challenge/pwn file in specific ways a few times in a row. If you get the permissions wrong, the game will reset and you can try again. If you get the permissions right eight times in a row, the challenge will let you chmod /flag to make it readable for yourself :-) Launch /challenge/run to get started!

## Solution

Round 1 of 8!

Current permissions of "/challenge/pwn": rw-r--r--

- the user does have read permissions
- the user does have write permissions

* the user doesn't have execute permissions

- the group does have read permissions

* the group doesn't have write permissions
* the group doesn't have execute permissions

- the world does have read permissions

* the world doesn't have write permissions
* the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": ---------

- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Answer ===> chmod a-rwx /challenge/pwn

Current permissions of "/challenge/pwn": ---------

- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": r--r--r--

- the user does have read permissions

* the user doesn't have write permissions
* the user doesn't have execute permissions

- the group does have read permissions

* the group doesn't have write permissions
* the group doesn't have execute permissions

- the world does have read permissions

* the world doesn't have write permissions
* the world doesn't have execute permissions

Answer ==> chmod a+r /challenge/pwn

Round 3 of 8!

Current permissions of "/challenge/pwn": r--r--r--

- the user does have read permissions

* the user doesn't have write permissions
* the user doesn't have execute permissions

- the group does have read permissions

* the group doesn't have write permissions
* the group doesn't have execute permissions

- the world does have read permissions

* the world doesn't have write permissions
* the world doesn't have execute permissions

Needed permissions of "/challenge/pwn": r--rwxrwx

- the user does have read permissions

* the user doesn't have write permissions
* the user doesn't have execute permissions

- the group does have read permissions
- the group does have write permissions
- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Answer ===> chmod go+wx /challenge/pwn

Round 4 of 8!

Current permissions of "/challenge/pwn": r--rwxrwx

- the user does have read permissions

* the user doesn't have write permissions
* the user doesn't have execute permissions

- the group does have read permissions
- the group does have write permissions
- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Needed permissions of "/challenge/pwn": r-xrwxrwx

- the user does have read permissions

* the user doesn't have write permissions

- the user does have execute permissions
- the group does have read permissions
- the group does have write permissions
- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Answer ===> chmod u+x /challenge/pwn

Round 5 of 8!

Current permissions of "/challenge/pwn": r-xrwxrwx

- the user does have read permissions

* the user doesn't have write permissions

- the user does have execute permissions
- the group does have read permissions
- the group does have write permissions
- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Needed permissions of "/challenge/pwn": r--r--rwx

- the user does have read permissions

* the user doesn't have write permissions
* the user doesn't have execute permissions

- the group does have read permissions

* the group doesn't have write permissions
* the group doesn't have execute permissions

- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Answer ===> chmod u-x,g-wx /challenge/pwn

Round 6 of 8!

Current permissions of "/challenge/pwn": r--r--rwx

- the user does have read permissions

* the user doesn't have write permissions
* the user doesn't have execute permissions

- the group does have read permissions

* the group doesn't have write permissions
* the group doesn't have execute permissions

- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Needed permissions of "/challenge/pwn": r-xr-xrwx

- the user does have read permissions

* the user doesn't have write permissions

- the user does have execute permissions
- the group does have read permissions

* the group doesn't have write permissions

- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Answer ===> chmod ug+x /challenge/pwn

Round 7 of 8!

Current permissions of "/challenge/pwn": r-xr-xrwx

- the user does have read permissions

* the user doesn't have write permissions

- the user does have execute permissions
- the group does have read permissions

* the group doesn't have write permissions

- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Needed permissions of "/challenge/pwn": r-xrwxrwx

- the user does have read permissions

* the user doesn't have write permissions

- the user does have execute permissions
- the group does have read permissions
- the group does have write permissions
- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Answer ===> chmod g+w /challenge/pwn

Round 8 of 8!

Current permissions of "/challenge/pwn": r-xrwxrwx

- the user does have read permissions

* the user doesn't have write permissions

- the user does have execute permissions
- the group does have read permissions
- the group does have write permissions
- the group does have execute permissions
- the world does have read permissions
- the world does have write permissions
- the world does have execute permissions

Needed permissions of "/challenge/pwn": ---rwxrwx

- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions

* the group does have read permissions
* the group does have write permissions
* the group does have execute permissions
* the world does have read permissions
* the world does have write permissions
* the world does have execute permissions

Answer ===> chmod u-rx /challenge/pwn

You've solved all 8 rounds! I have changed the ownership
of the /flag file so that you can 'chmod' it. You won't be able to read
it until you make it readable with chmod!

Current permissions of "/flag": ---------

- the user doesn't have read permissions
- the user doesn't have write permissions
- the user doesn't have execute permissions
- the group doesn't have read permissions
- the group doesn't have write permissions
- the group doesn't have execute permissions
- the world doesn't have read permissions
- the world doesn't have write permissions
- the world doesn't have execute permissions

Answer ===> chmod a+r /flag

cat /flag
