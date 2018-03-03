# Reminder App
This project integrated the *Positivo Challenge*, a research and development project carried out by the *University of Brasília* (UnB) in partnership with *Positivo*.

### Features
The features present in this release are:

![Feature Model](https://i.imgur.com/nmtGwK7.png)


# Steps to run the project
To run this project it is necessary to use the Eclipse IDE - we are using the [Eclipse Neon for Android Developers](https://www.eclipse.org/downloads/packages/eclipse-android-developers/neonm6). Once you have the IDE installed, the steps that must be followed to import the project are:

1. Open the Eclipse IDE and go to **Help -> Install New Software** <br />
1.1. Install the [DeltaJ 1.5](https://www.tu-braunschweig.de/isf/research/deltas/) plugin: https://www.isf.cs.tu-bs.de/cms/research/deltas/downloads/plug-in/

2. Now go to **Window -> Android SDK Manager**<br />
2.1. Select options to install **Android API 19**.

3. *This step is optional*. To create a virtual device, go to **Window -> Android Virtual Device Manager** and create the device with the following configuration: <br /> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Create a Virtual Device to Android](https://i.imgur.com/nGM9z8u.png)

4. To import the project go to **File -> Import -> Maven -> Existing Maven Project** and select the project in the directory where it was cloned;

5. To run the project click **Properties -> Java Builder**  and verify that the following parameters are configured: <br /> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Java Compiler Configuration](https://i.imgur.com/z30LeVx.png)

6. After, right click on the project and then on **Run As -> Run Configurator -> Android Application -> New** and make the following settings: <br /> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Settings to Run Configurator](https://i.imgur.com/3oQcgx8.png)

7. *This step is optional because it is intended for anyone who wants to modify the project*. Now right click on the project and go to **SPL** and enable **Enable project specific settings** and make the following settings: <br />
7.1. In the **Source Folder** option: <br /> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![Settings to Source Folder](https://i.imgur.com/53MyHiO.png)

8. To generate a product, go to the **Project -> Build Project** menu and select this project. Then select the desired product and wait for the source code to be generated.

9. Finally, run the application on the virtual device or on your own device.

That is all.

Leomar Camargo, [leomarcamargodesouza@gmail.com](mailto:leomarcamargodesouza@gmail.com).
