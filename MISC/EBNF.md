The Extended Backus Naur Form is a notation to describe the syntax of complex grammars.

5 simple rules

1. literal     => anything written without the special symbols should be written/present as is <br>
2. \<mandatory value>  => placeholder for a single mandatory value, the value is going to be literal, but what exact literal is up to choice.<br>
3. \[optional value]   => the value inside might be written 0 or 1 times<br>
4. choice1 | choice2 => either one of those values can be put here once<br>
5. {value}           => the value inside can be repeated 0 to infinite times<br>