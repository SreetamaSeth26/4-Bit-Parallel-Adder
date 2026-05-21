# 4-Bit-Parallel-Adder
A 4-bit parallel adder adds two 4-bit binary numbers and a carry-in by chaining four full adders (FA) in series. The carry-out of each stage ripples into the carry-in of the next, producing a 4-bit sum and a final carry-out.
Module Structure

fa — 1-bit Full Adder (the basic building block)
parallel_adder — chains FA1 → FA2 → FA3 → FA4 to add A[3:0] + B[3:0] + Cin

Full Adder Truth Table
abcinsumcout0000000110010100110110010101011100111111
Testbench Results
CinABSumCoutDecimal000000000000000 + 0 = 0000110101100003 + 5 = 80111100010000115 + 1 = 161101001010000110 + 5 + 1 = 16
