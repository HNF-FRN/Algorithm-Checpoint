# Algorithm-Checkpoint

ALGORITHM checkpoint
var
ch[]: string; 
i : integer;
lenght : integer;
words : integer;
vowels : integer;

Begin

write "Enter a string: ";
read (ch);
i <-- 0;
lenght <-- 0;
words <-- 0;
vowels <-- 0;

while (ch[i] != '.') do {
lenght <-- length + 1;

    if (ch[i] == ' ') then {
        words <-- words + 1;
    }

    if (ch[i] == 'a' or ch[i] == 'e' or ch[i] == 'i' or ch[i] == 'o' or ch[i] == 'u') then {
        vowels <-- vowels + 1;
    }

    i <-- i + 1;
    }

words <-- words + 1; // for the last word
lenght <-- lenght + 1;// top count the last dot

write "Length of the string: ", lenght;
write "Number of words: ", words;
write "Number of vowels: ", vowels;

End
