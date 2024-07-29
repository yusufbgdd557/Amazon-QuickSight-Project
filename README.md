# Netflix Data Visualization with Amazon QuickSight

This project demonstrates how to visualize Netflix data using Amazon QuickSight. The dataset is stored in an Amazon S3 bucket and connected to QuickSight for creating interactive visualizations.

## Project Overview

This project involves the following steps:
1. Uploading the Dataset
2. Creating a QuickSight Account
3. Connecting the Dataset to QuickSight
4. Creating Visualizations
5. Using Filters
6. Setting up a Dashboard

## Steps

### Step 1: Upload Dataset to S3
Upload the Netflix dataset file and `manifest.json` to your Amazon S3 bucket. 

![1](https://github.com/user-attachments/assets/00e97921-6a97-495c-b879-081ab5d0c1a3)

Edit the `manifest.json` file by replacing the placeholder S3 URI with the actual S3 URI of your dataset file. This step ensures that QuickSight can correctly locate and access the dataset. Here's an example of what the `manifest.json` file should look like:

```json
{
  "fileLocations": [
    {
      "URIPrefixes": [
        "s3://your-bucket-name/path-to-your-dataset-file/"
      ]
    }
  ],
  "globalUploadSettings": {
    "format": "CSV",
    "delimiter": ",",
    "textqualifier": "\"",
    "containsHeader": "true"
  }
}
```

### Step 2: Create a QuickSight Account
Create a QuickSight account. (Don't forget to delete your QuickSight account if you don't want to be charged after the free trial ends!)

![2](https://github.com/user-attachments/assets/6e861e94-41f4-4f26-9734-f846b8d447dc)

### Step 3: Connect the Dataset to QuickSight
Connect the S3 bucket to QuickSight by navigating to the Dataset page. The `manifest.json` file acts as a guide for QuickSight to access and visualize the dataset.

![3](https://github.com/user-attachments/assets/c928e420-bf12-49a3-9771-92d05e5747c9)

### Step 4: Create Visualizations
Drag relevant fields from the dataset to the AutoGraph space in QuickSight. For example, create a graph by placing the release year on the y-axis and using the type (i.e., movie or TV show) as the grouping variable.

![4](https://github.com/user-attachments/assets/1b8bab30-6206-4440-afb4-89a6c6373538)

### Step 5: Using Filters
Apply filters to refine the dataset. For instance, display only movies released after 2015 or exclude certain genres. This helps focus on specific criteria and analyze trends more effectively.

![5](https://github.com/user-attachments/assets/f5e8380a-3ec5-4801-a569-f635dd8829d8)

### Step 6: Setting up a Dashboard
Edit the titles of your graphs and charts. You can export your dashboard as PDFs by publishing it and then generating and downloading it as a PDF.

![7](https://github.com/user-attachments/assets/a007e176-1105-47d3-b72c-e9fa245c2a51)
