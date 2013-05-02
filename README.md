mysqldump_filter
================

filter mysqldump output - include and exclude tables, plus sundry others

USAGE
-----
        mysqldump_filter --exclude=table1[,table2,table3]
        mysqldump_filter --exclude_data=table1[,table2,table3]
        mysqldump_filter --include=table1[,table2,table3]
        mysqldump_filter --include_data=table1[,table2,table3]
        mysqldump_filter --include_structure=table1[,table2,table3]
        mysqldump_filter --definer_current

    text read on stdin is filtered and printed to stdout

    multiple --include* options can be combined, as can multiple --exclude*
    options.

    --include* options and --exclude* options cannot be combined with each
    other

    --definer_current will change the DEFINER of any views to CURRENT_USER,
    and can be combined with --include and --exclude options

