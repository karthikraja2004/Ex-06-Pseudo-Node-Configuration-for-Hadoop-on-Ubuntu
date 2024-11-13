# Ex-07-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop
<img width="364" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/35fc604a-b0ab-40fc-8c0a-2ee10d501156">


2.	Install java1.8 in folder /usr/local

<img width="364" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/53b94ac6-7ebc-42a4-ae89-b206f6ea559a">

3.	Install Hadoop

<img width="363" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/5cdaa399-3e75-41eb-9a28-1178af495a4f">

4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file
<img width="398" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/14ed0431-523e-4548-9988-7338ff06fca2">

 
5.	Set hadoop environment variables: Include the following lines /etc/profile file

<img width="390" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/3dbb2d25-facb-44df-94d7-9f4268806c23">

6.	Run the.bashrc & profile files from the $ prompt for updating the changes
<img width="388" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/e01c3ad1-d0ca-4364-892f-f261a00bfd3c">
<img width="388" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/7d364a7e-01d2-4679-b324-ff983d34a103">





$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file
<img width="379" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/90527341-0e60-43b5-9349-20ea45903852">


b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)
<img width="378" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/da9b7cd6-b246-41bc-aca4-ac029d6356ce">


 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags
<img width="366" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/5c29ab4d-7a7a-441a-b7fe-f614b62f19b9">


c)	mapred-site.xml
 <img width="381" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/20ddec48-5047-4590-8571-002d85543bc2">


Include the following lines in mapred-site.xml file
 <img width="378" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/9e099f76-bf5d-4db0-8583-9a3931681b21">


d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file
<img width="374" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/6f8b6f3c-ea68-4c74-a516-eb8c6681196c">


e)	yarn-site.xml
Include the following lines in yarn-site.xml file
<img width="369" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/21a54b26-ce93-4cc0-aeda-114970a430f1">

8.	Format the Hadoop File system implemented on top of the local file system using
<img width="367" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/0627f010-0111-413f-b790-022f5a0d5127">

9.	Start Hadoop using

<img width="374" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/7b468721-de8b-4ca6-a97b-81b6b3637ab4">

Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:
<img width="371" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/6f86cd24-c12c-45f9-8191-2de8e70ec27e">


11.	Create a directory ‘/input’ in HDFS
<img width="383" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/c6fb940a-5d5f-4f65-87dd-7cb4999619f5">


12.	Copy the input files into the distributed file system
<img width="404" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/f9702a08-3a7b-46f4-8f88-5cf3e631eb48">

13.	Run some of the examples provided
<img width="394" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/e5b714d9-8141-4740-a01b-e88b50eee1a5">


14.	Examine the output files
<img width="399" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/95b8f297-a44b-4601-bff7-a99a95567fca">


Copy the output files from the distributed file system to the local file system and examine them:
<img width="373" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/13ff9827-47ab-42a1-af60-124d1cc05959">


or
View the output files on the distributed file system
<img width="373" alt="image" src="https://github.com/1808charitha/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/132996838/ab6182fa-5119-48ea-8e7f-98dcc7f80aa3">

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
