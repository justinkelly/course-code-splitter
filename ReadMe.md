=========
### What

  * Split uni course codes into space seperated format based on rules ie HAH101 becomes 'HAH 101'

### Why 

  * I needed a way to get thousands of our course code ie. HAH219 into space seperated format - so people could search search for them ie. 'HAH 219'

### How to run
Put your course codes in course_codes.txt?

Run
    ./course_code_splitter.pl

Then you'll be prompted for a output file name

    Please enter an output file name, default is split_course_codes.txt

This will now convert the contents of the $course_codes_file into space separated format ie. HAH101 becomes HAH 101

### Course codes

Our course codes look similar to the below example - We have about 10 different formats and it you review the search logs you will see how the students search for cource material using different formats
ie. for course EXT003 they will search EXT 003

This script reformats the non-spaces codes into the spacing format that students search on and adds them to the userSynonyms file

    EXT003
    EXT004
    EXT005
    EXT006
    EXT007
    EXT008
    G0046CE01
    G0046CE02
    G0046CE03
    G0046CE04
    G0046TD019
    G0046TD020
    G0046TD021
    G0046TD022
    G0046TD22P
    HAA101N
    HAA102N
    HAA103N
    HAA119
    HAA184T
    HAA185T
    HAA201N


### Adding your course codes

You can your course codes into the course_codes.txt file in a non-spaced format - such as

    G0046TD022
    G0046TD22P
    HAA101N

