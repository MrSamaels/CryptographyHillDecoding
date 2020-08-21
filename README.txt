Program wasn't optimized and was developed for games with Hill algorithm

Simple decoder for Hill algorithm with matrix 7x7 for text in Russian language
Main idea is in standard letter frequency distribution in russian text. Most common letters are 'а' and 'o', so on frequency distribution of this letters we can find crypto keys, that could be used on encrypting.
After finding crypto keys we can recover matrix for decode. 

For example in program we found keys:
cnt 14 KEY: 0 5 15 3 14 3 22

cnt 12 KEY: 0 11 2 19 6 19 5

cnt 26 KEY: 0 15 14 9 11 9 4

cnt 12 KEY: 4 4 27 0 0 30 18

!!!Success!!! cnt = 26
 KEY: 4 11 12 25 3 16 3

cnt 7 KEY: 4 11 12 25 3 16 4

cnt 11 KEY: 5 6 15 8 27 20 27

cnt 7 KEY: 8 30 28 4 8 22 15

cnt 9 KEY: 16 11 12 19 16 15 10

!!!Success!!! cnt = 27
 KEY: 16 15 27 15 21 28 14

cnt 7 KEY: 16 15 27 15 21 28 15

cnt 24 KEY: 16 28 20 18 6 19 13

cnt 12 KEY: 17 5 28 0 5 17 30

cnt 23 KEY: 17 27 19 13 24 12 21

cnt 9 KEY: 20 4 25 7 23 16 24

cnt 11 KEY: 20 11 26 11 3 4 2

cnt 5 KEY: 23 17 16 12 20 19 18

cnt 10 KEY: 24 1 0 15 20 22 16

cnt 12 KEY: 25 20 23 5 24 1 6

!!!Success!!! cnt = 24
 KEY: 26 4 10 0 4 26 24

cnt 7 KEY: 26 4 10 0 4 26 25

cnt 9 KEY: 26 30 13 28 15 26 24

cnt 26 KEY: 28 28 3 0 0 24 2

cnt 8 KEY: 29 26 16 24 30 15 3

After recovering we got matrix:
KEY:  17  27  19  13  24  12  21
KEY:  4   11  12  25  3   16  3
KEY:  26  4   10  0   4   26  24
KEY:  16  28  20  18  6   19  13
KEY:  16  15  27  15  21  28  14
KEY:  0   15  14  9   11  9   4
KEY:  28  28  3   0   0   24  2

We've got a story of Veresaev 'В сухом тумане'

