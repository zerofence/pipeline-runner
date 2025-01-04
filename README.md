# pipeline-runner

connections:
   
# steps
steps:
    - name: Step 1
      tasks:
      - name: ExecuteQueryTask@1
        query: |
            Select * from Table1
      - name: ExportTask@1
        format: xlsx
    - name: Step 2
      tasks:
      - name: UploadSFTPTask@1
        key: ''
        source: ''
        destination: ''
