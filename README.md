# utl_two_columns_with_the_same_name
Two columns with the same name. Keywords: sas sql join merge big data analytics macros oracle teradata mysql sas communities stackoverflow statistics artificial inteligence AI Python R Java Javascript WPS Matlab SPSS Scala Perl C C# Excel MS Access JSON graphics maps NLP natural language processing machine learning igraph DOSUBL DOW loop stackoverflow SAS community.

    Two columns with the same name

    github
    https://github.com/rogerjdeangelis/utl_two_columns_with_the_same_name

    inspired by
    https://communities.sas.com/t5/SAS-Communities-Library/SQL-Allows-Multiple-Columns-with-Same-Name/ta-p/475974


    INPUT
    =====

      sashelp.class

    EXAMPLE OUTPUT
    --------------

       WORK.WANT total obs=19

           NAME       NAME

           Alfred     Alfred
           Alice      Alice
           Barbara    Barbara
           Carol      Carol
        ...


    PROCESS
    =======

       options validvarname=upcase;
       proc sql;
         create
           view want as
        select
          name as name
         ,name
        from
          sashelp.class
       ;quit;


    OUTPUT
    ======


      WORK.WANT total obs=19

        NAME       NAME

        Alfred     Alfred
        Alice      Alice
        Barbara    Barbara
        Carol      Carol
        Henry      Henry
        James      James
        Jane       Jane
        Janet      Janet
        Jeffrey    Jeffrey
        John       John
        Joyce      Joyce
        Judy       Judy
        Louise     Louise
        Mary       Mary
        Philip     Philip
        Robert     Robert
        Ronald     Ronald
        Thomas     Thomas
        William    William

