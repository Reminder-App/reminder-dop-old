# Reminder App
This project integrated the *Positivo Challenge*, a research and development project carried out by the *University of Brasília* (UnB) in partnership with *Positivo*.

### Features
The features present in this release are:

![Feature Model](https://i.imgur.com/ENMbZFT.png)


# Steps to Generate a Product
To run this project it is necessary to use the Eclipse IDE - we are using the [Eclipse Neon for Android Developers](https://www.eclipse.org/downloads/packages/eclipse-android-developers/neonm6). For the project to work, make sure that you have the following components installed:

* Open the Eclipse IDE and go to **Help -> Install New Software** and install the [DeltaJ 1.5](https://www.tu-braunschweig.de/isf/research/deltas/) plugin: https://www.isf.cs.tu-bs.de/cms/research/deltas/downloads/plug-in/;

* Install and configure the [Hepheatus](https://github.com/hephaestus-pl/hephaestus-base);

In order for the final product to be generated, the following steps must be performed.

### First Step

This first step is to generate the java source code for the desired product. It is important to note that importing this project into the Eclipse IDE will contain errors due to the preprocessing directives present in the *.xml* files that corresponds to the graphical interface of the Reminder App - this part will be handled in the **Second Step**.

1. With the DeltaJ plugin installed, import the project into the Eclipse IDE: <br />
1.1. **File -> Import -> Existing Android Code Into Workspace**. **IMPORTANT**: After the import, ignore the errors in the product line, because we first used Eclipse to generate the java source code;

2. Open the **Project Explorer** and go to **spl-info -> Reminder.spl**;

3. Go to menu **Project -> Clean**. After that, it will open a DeltaJ Plugin window so that a product is generated: <br /> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![DeltaJ Products do select](https://i.imgur.com/wekIELK.png)

4. Close the Eclipse IDE.

### Second Step

To continue, all steps in step 1 must have been successfully executed. This step will be responsible for managing the graphical interface variability of the Reminders app. For this, the Hepheatus tool is used.

1. In the directory for this project, open the **spl-config** folder. Then open the file **project.properties** and replace the *&lt;directory-where-this-repository-is-cloned&gt;* tag as requested. <br />
1.1. Then change the value of *instance-model* according to the product generated in the First Step instruction 3. **IMPORTANT**: an error will occur if the product selected in this step is direct from the one generated in the First Step;

2. Open the workspace where the Hepheastus tool is installed. Then go to **hephaestus-sb/bin** and run the *hepheastus* file. <br />
2.1. After running hephaestus, the following screen will appear: <br /> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Hephaestus Tool](https://i.imgur.com/OvtqDMh.png)

3. Enter the command *start*. Then enter the **absolute path** where the *project.properties* file is located and then confirm;

4. Navigate to the target directory that was entered in the *projects.properties* file.

5. Open the terminal and enter the command below. Remember to replace *&lt;hephaestus-workspace-path&gt;* with its corresponding value: <br /> *java -jar &lt;hephaestus-workspace-path&gt;/hephaestus-pp/bin/antenna-pp.jar files.pp build.lst --drop-lines*

6. After, the generated product design is fully configured. So import it into the Eclipse IDE or Android Studio and emulate the Reminder app.


##### It's important to know

* Keep the Eclipse IDE closed by following the instructions in **Second Step**;
* Using the Eclipse IDE in **First Step** is necessary because of the DeltaJ plugin. However, the product generated after performing the instructions in **Second Step** may be important to the Eclipse IDE as well as to Android Studio.

That is all.

Leomar Camargo, [leomarcamargodesouza@gmail.com](mailto:leomarcamargodesouza@gmail.com).
