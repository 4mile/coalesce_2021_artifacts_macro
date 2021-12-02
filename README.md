# coalesce_2021_artifacts_macro

create_artifact_resources macro will create the stage and table for the json files.  To execute this macro `dbt run-operation create_artifact_resources`

upload_artifacts macro will put the file into the target and then copy the files into a table.  To execute this marco make sure to use the appropriate argument to pick up the correct json file. `dbt run-operation upload_dbt_artifacts --args '{filenames: [run_results]}' `
