## Compiler_Construction
- This project comprises of a working compiler constructed for a custom-defined, C-like langauge _ErPlag_. The language has been designed for the purposes of the project of the 2022-2023 offering of the course CS-F363 (Compiler Construction). The specifications about the ErPlag language can be found in the _language_specifications.pdf_ document. All theoretical modules of a compiler have been included in our project: lexical analyser, syntax analyser (parser), semantic analyser, and code generator.
- You may try the compiler by following these steps:
    - On a Linux-based terminal, navigate to the project directory, and then execute:
      ```
      > make
      ```
    - This should compile the project. You must now execute the following command:
      ```
      > ./compiler <testcase_file.txt> <generated_code.asm>
      ```
    - In the above command <testcase_file.txt> could be replaced with any of the *t[1-6].txt, ts[1-10].txt, or c[1-10].txt* files. Note that many of them contain lexical, syntactic and semantic errors for testing the robustness of the compiler; hence, proceed liberally with the testing.
    - <generated_code.asm> is the x86 generated executable code for the corresponding ERPLAG code. Any other name could be given to this file, while ensuring the proper extension .asm is used.
    -  To run the generated code and see its output (code will only be generated in case the input file was lexically, syntactically, and semantically correct), execute the following command:
        ```
        > nasm -felf64 <generated_code.asm> && ld code.o && ./a.out
        ```
_Note: This project has been developed using **gcc version 11.3.0 ~ ubuntu 22.04** and **nasm version 2.14.02**. Please ensure compatibility with these versions on your system prior to testing._
- Finally, cheers and shoutout to my teammates **_Harsh, Hrishikesh, Antriksh, and Shashank_** for their valuable contributions to the project. It has been a wonderful journey and an enriching experience working with them on this project.
