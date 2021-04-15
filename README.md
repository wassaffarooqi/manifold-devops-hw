# manifold-devops-hw

## Homework Problem

### BACKGROUND

Our goal is to build an endpoint for a hypothetical vendor to send us user data in slightly different formats; The design is in place but needs to be automated.

### Assignment

Produce the Terraform code needed to support a Dev Team tasked with the following below.  Feel free to create a design doc of what you are thinking, as well as ask any questions that will help clarify any of this design.  In addition to the terraform code, also include documentation to help the developers run and deploy the terraform themselves.

This is an image of the design the developer wants to implement:

![Appflow](https://github.com/manifoldai/manifold-devops-hw/blob/542a705a3a6746b9872c9280200d156d0064f044/images/DevOps%20Homework.png)

The dev team assignment calls for python code, supplied is a stub file.  The stub file is fine to use for the Lambda function.

### What Manifold Will Assess

These take homes allow us to give candidates the ability to show a breadth of what they know.  We undersatnd that these take homes can be a substantial effort, so we ask that you prioritize and do as much as you think needs to be done to show what you are able to do.  We have no time constraints on how long someone should spend; candidates who can spend more time allow us to get a better picture of who they are earlier in the process.

We use this assigment to assess how a candidate learns new technologies, write documentation (we have a strong reading / writing culture), and how they write code.  We very much like these assignments to reflect how working at Manifold is, so feel free to reach out if you have questions or want to share any early notes before implementation if it will help you.  

If you need to prioritize how much time you spend, please focus on writing up the design and approach, the readme for how someone will use this, and a subset of the terraform code that you think will give us a good picture of how you write and organize your code.  

After the assignment is done, email a zip file with the code, and we'll schedule a 60-90 minute review to walk through the problem and your solution.  In this, we'll also ask some questions about what you think of the developer solution and how it will work at different scales, and what you might suggest doing differently.  We will also ask how you might consider logging, monitoring, and alerting for this solution - you can prepare some notes ahead of time in the design doc, or even choose to implement something if you have a practiced pattern that you enjoy.  


Bonus Points:  Actually implement the python code and associated tests needed to make the below assignment work.  

### Dev Teams Assignment needing support

Please make an API endpoint deployed on AWS that will take in any random JSON data structure. From inside the structure, it should pull out first_name, middle_name, last_name, and zip_code, and store that data in S3.  The JSON structure could have these fields at any cardinality.  Some examples:

```
{
  "first_name": "First",
  "last_name": "Last",
  "middle": "K"
  "zip_code": "02115"
}
```

```
{
  "names": [ 
      {
      "first_name": "First",
      "last_name": "Last",
      "middle": "K"
      }
    ],
 "zip_code": "02115"
}
```



Make this using API Gateway and Lambda (with python code).

After the data is stored in S3, make a queryable table with AWS Glue and be able to present it for querying using Athena. 



