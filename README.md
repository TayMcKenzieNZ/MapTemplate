<div align="center">

# MapTemplate 🗺️

</div>

MapTemplate is a resource template designed to simplify the conversion of GTA 5 single player maps to FiveM. By downloading MapTemplate, you'll have everything you need to seamlessly convert maps for use in your FiveM server.

## Getting Started

1. **Download the MapTemplate Resource**: Simply download the MapTemplate resource from this repository.

2. **Explore the Stream Folder**: Inside the MapTemplate resource, you'll find a stream folder containing various subfolders, each representing a specific type of file related to the map conversion process.

   - **ybn folder**: Place all map ybn collision files here.
   - **ymap folder**: Place all ymap files here.
   - ... (and so on for other types of files)

## Custom Props and ytyp Files

If the map you've downloaded includes custom props, you may also find a ytyp file. To incorporate custom props into your map:

1. **Insert the ytyp File**:
   - Locate the ytyp file and place it in the "ytyp" subfolder within the stream folder.

2. **Modify fxmanifest**:
   - Open the fxmanifest file and uncomment the line:
     ```lua
     -- data_file "DLC_ITYP_REQUEST" "ytyp_name_here.ytyp"
     ```
   - Replace `ytyp_name_here.ytyp` with the actual name of the ytyp file.

## Configuring FiveM

Once you've organized the necessary files and set up the ytyp integration (if applicable):

1. **Edit your server.cfg**:
   - Open your `server.cfg` file.

2. **Add Map Resource**:
   - Add the following line to ensure the map resource in your server:
     ```plaintext
     ensure mapnamehere  # Replace "mapnamehere" with the actual map resource name (e.g., dnxnewsenoraroad)
     ```
