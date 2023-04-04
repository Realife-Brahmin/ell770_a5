Rules:
1. Bus 1 must have a shunt element (connecting to the reference), either as part of a branch connecting it in systemXXX_branchData.xlsx, or a separate shunt element in systemXXX_busData.xlsx.
2. Every subsequent row of systemXXX_branchData.xlsx may contain upto one new bus (hitherto not part of any other previously defined branch). But both buses i and j MUST NEVER SIMULTANEOUSLY BE NEW. Violation of this rule would break this program.

To run:
1. Run a5_01_main.mlx. You may define testCase='003_1'/'003_2'/'004_1'/'004_2' for prespecified systems in the prespecified_systems. Alternatively, you may define your own system specification in two new excel files (names should match the format of prespecified systems) and modify the read file name in the readtable() command.

Output:
1. Outputs (excel file) can be found in outputs folder.

Notes:
1. There is  no case3 script because it is always avoided in the algorithm while using case1.