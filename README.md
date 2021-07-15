_____________INTRODUCTION_____________<br/>

This work on the Kibiku forest was done as part of the MIDST NRM project piloted by the Kenya Space Agency, using satellite imagery on the Google Earth Engine platform to 
analyze raw satellite imagery into high level land cover classification products. This guide will enable new as well as intermediate and advanced users of the Google Earth Engine 
platform to run the scripts in this repository and view the products.<br/>
The scripts contain comments that highlight a step by step of the process followed in analysing and generating products for the aberdare forest.

______________RUNNING THE SCRIPTS______________<br/>

This process will consist of six steps as follows:<br/>
1.) Accessing GEE<br/>
2.) Downloading the files<br/>
3.) Ingesting the assets into the GEE platform<br/>
4.) Paste the script code onto GEE and convert imports<br/>
5.) Importing the assets/ shapefiles into the script<br/>
6.) Run the script to view products<br/>

To better understand the script and how to do Machine learning with the google earth engine platform, refer from [Supervised classification in Earth Engine](https://developers.google.com/earth-engine/guides/classification)

_______________1.) ACCESSING THE GEE PLATFORM_______________<br/>
The GEE code editor platform is accessed [here](https://code.earthengine.google.com). It requires the users to have a [google account (Gmail)](https://mail.google.com). For new GEE users, it will prompt them to request for access. The response varies in duration.
For more information and a detailed introduction to the platform, refer to the [GEE playground](https://developers.google.com/earth-engine/guides/playground).

_______________2.) DOWNLOADING THE FILES____________________<br/>

![image](https://user-images.githubusercontent.com/75077556/125576767-07d47298-d2ca-44e6-b3df-b837643adba2.png)<br/>
Click on the 'Clone' button at the top of this page, then click on 'Download ZIP', as shown in the image above. Once the zipped file is downloaded, extract the files to a location of your choice. You can open the folders to view the files. There are a number of different files in the folder; there is the script file containing the GEE code and the sub-folders containing the assets (shape files).

_______________3.) INGESTING THE ASSETS/ SHAPE FILES ONTO THE GEE PLATFORM_____________<br/>

![image](https://user-images.githubusercontent.com/75077556/125578391-7ab741aa-633a-4f5b-92dd-ab10c8ea1425.png)<br/>
Once you have been able to access the GEE code editor platform from step one above, on the left hand panel, click on the 'assets' tab as shown in the image above, then click 'NEW'. Under 'Table Upload' click on 'Shape files'.<br/>
![image](https://user-images.githubusercontent.com/75077556/125578723-c0d0d13e-62bc-485d-b3b6-36aa4805cc1e.png)<br/>
As shown above, the 'Upload Shapefile' dialog box will appear as shown above. Click on the 'SELECT' button and navigate to the folder containing your shape files. Select all the files contained within the shapefiles folder, and put in a name of your choice, for the asset. Scroll down the dialog box and click 'UPLOAD'. Wait for the upload to complete and your asset will appear under the assets tab with the name you set for it. You will need to do this for the 'AOI_shapefile' and the 'Sample_data_shapefile' in the aberdare project folder. For more details on asset management on GEE, refer from the [GEE asset manager](https://developers.google.com/earth-engine/guides/asset_manager)

_______________4.) PASTE THE SCRIPT CODE ONTO THE PLATFORM___________________________<br/>

From within the project folder, open the 'script.js' file using a text editor of your choice. You will see a huge collection of almost incomprehensible code. Not to worry, as the earth engine code editor has the ability to manage the huge code. Select and copy all the code from the text editor and paste it onto the GEE code editor platform. Scroll to the top of the code editor where you will see the geometry imports with their raw definitions. When you place your cursor above the code, you will see a prompt at the bottom. It lists all the geometry objects defined and gives you an option to 'convert to import records' as highlighted below. Once you select the option, your imports will be organized on your code editor.<br/>
![image](https://user-images.githubusercontent.com/75077556/125584368-d970818f-b5f8-49d7-a84e-c02744911aeb.png)<br/>

_______________5.) IMPORT THE ASSETS/ SHAPE FILES INTO YOUR SCRIPT___________________<br/>
![image](https://user-images.githubusercontent.com/75077556/125596583-ffe2719c-a354-4737-aec4-e630dea8d829.png)<br/>
As shown in the image above, once your imports are in an organized fashion (import records), you will have to replace the highlighted imports with the assets you ingested in step 3 above; the 'kibikuarea AOI_shapefiles'. Name the imports with the same names in the existing imports, i.e.<br/>
-'AOI'<br/>

![image](https://user-images.githubusercontent.com/75077556/125587500-92fe80ac-13b9-4648-8571-54accc9e1041.png)<br/>
Use the bucket icon on the left hand side of the import, as shown in the image above, to delete the existing import. The icon appears once you hover your cursor on the left side of the imports.<br/>
![image](https://user-images.githubusercontent.com/75077556/125588164-7a1a844b-f46d-4a6d-824e-03b0b59346c9.png)<br/>
Use the arrow icon to the right hand side of the asset you want to import into your script, to import the asset into your script, in the 'assets' tab as shown in the image above.

_______________6.) RUN THE SCRIPT TO VIEW PRODUCTS____________________________________<br/>

At this point you should now be able to run the script and view the products. For more information and details, refer from the [Google Earth Engine Official Documentation](https://earthengine.google.com/).
