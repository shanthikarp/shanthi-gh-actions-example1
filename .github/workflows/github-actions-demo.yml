name: Github actions workflow
on: 
  push:
  pull_request:
    branches: 
    - main
  schedule:
      - cron: '15 6 * * 0'  
  workflow_dispatch: 
  workflow_call:
   outputs:
      workflow_output1:
        description: " Printing the event triggered the workflow"
        value: ${{github.event.type}}
jobs:
  job1:
    name: "Build"
    runs-on: ubuntu-latest
    outputs:
      output1: ${{ github.event.type }}
    steps:
      - name: step1
      - uses: actions/checkout@v4
      - name: step2
        run: echo  ${{ github.ref }}
             echo ${GITHUB_WORKFLOW}
       
     
    
    

      
