# Constellation Plots in KNIME: An Automated Scaffold-Based Workflow for Interactive Chemical Space Visualization
## Specifications
The workflow was implemented using the KNIME Analytics Platform (v. 5.4.2), which can be downloaded for free at knime.com/downloads. While most steps utilize KNIME Base Nodes, others require specific free extensions, such as:

-KNIME Statistics Nodes (Labs)

-RDKit Nodes Feature

-KNIME SVG Support

The workflow is available in .knwf format, the standard file type for KNIME workflows.

## Download and Import Guide
Once you have downloaded the desired workflow, you can import it into the KNIME Analytics Platform by following these steps:

Open the KNIME Analytics Platform.

Click on the Home button, then navigate to Local Space.

Click the Import Workflow button, locate the .knwf file in your downloads folder, and click Open.

The workflow is now ready to use!

[!IMPORTANT]
Since the workflow requires specific nodes not included in the standard installation, a "Missing extensions" pop-up will appear. Please confirm the installation to allow KNIME to automatically download and install the required nodes.

#### Extra Information
Users can also manually install new nodes through the Install section located in KNIME’s main interface.

## Chemical dataset requirements
The workflow requires from the user a chemical database in any of the following formats: CSV, Table, XLSX, or SDF. The input file must include three columns: 1) a column with the compound's chemical linear representation (such as SMILES, SMARTS, or InChiKey); 2) a column with a numerical experimental or calculated property (for instance, a biological property such as activity or a physicochemical or molecular property property), and 3) a column with the molecule name or an identifier.
To ensure accurate calculations and visualization, if a biological property - such as activity - is selected, all values must be expressed in consistent units. Mixed unit will result in incorrect standard deviation and mean activity values.
