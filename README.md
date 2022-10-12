# Dataverse Uploads

## Contact Information

- Principal Investigator: Peter Sorger, Laboratory of Systems Pharmacology, Harvard Medical School (`peter_sorger@hms.harvard.edu`)
- Data Manager: Sarah Arena, Laboratory of Systems Pharmacology, Harvard Medical School (`sarah_arena@hms.harvard.edu`)

## Harvard Dataverse Directory Structure

First, expand the `dataverse_files.zip` archive. Then, move or copy `STORY-NAME.zip` to `STORY-NAME`. Finally, expand the `STORY-NAME.zip` archive.

The unextracted directories will appear as follows:

```
├── README.md
'── STORY-NAME
  ├── STORY-NAME
  |   ├──- channel-group
  |   |   '── image tiles (.jpg)
  |   ├──- masks (optional)
  |   |   '── mask-group
  |   |      '── mask tiles (.png)
  |   '──- visdata (optional)
  |       '── visualizations (.csv)
  |── index.html
  '── img (optional)
      '── illustrations (.png)
```
## Archive Extraction 

Due to the large number of separate JPEG/PNG files in a minerva story, we have combined the JPEG/PNG files into a single ZIP archive for easier management within Dataverse. To unpack the JPEG/PNG files into the proper location for correct functioning of the story, download and unzip the following zip archives into the corresponding directories:

- Unzip [`lin-2021-viz-97.zip`][0] within `lin-2021-viz-97`
- Unzip [`lin-2021-reg_96_97.zip`][1] within `lin-2021-reg_96_97`
- Unzip [`gaglia-2020-0813.zip`][2] within `gaglia-2020-0813`
- Unzip [`gaglia-2020-gemm-lung.zip`][3] within `gaglia-2020-gemm-lung`

The zip archive will be created a subdirectory with the same name as the parent, ie:

- `lin-2021-viz-97/lin-2021-viz-97`
- `lin-2021-reg_96_97/lin-2021-reg_96_97`
- `gaglia-2020-0813/gaglia-2020-0813`
- `gaglia-2020-gemm-lung/gaglia-2020-gemm-lung`

## File Descriptions

- .zip: .zip archive containing JPEG/PNG pyramid files for multiple zoom levels to be assembled by a Minerva Story. 
  - The JPEG files are rendered from fluorescence ome.tif images.
  - Optionally, PNG files are rendered segmentation masks from ome.tif images.
  - Optionally, CSV files are rendered to chart visualizations associated with the data.
- index.html: An html file generated from markdown files to publish the story online.
  - The HTML contains a JSON configuration output to control channel groups and waypoints.

## File Naming Structure

- JPEG: channel-group/tile-location.jpg (e.g., `AKT_34__AKT/0_0_7.jpg`)
- PNG: mask-group/tile-location.png (e.g., `TNP097_21types/0_0_7.png`)

[0]:https://dataverse.harvard.edu/file.xhtml?fileId=6561382
[1]:https://dataverse.harvard.edu/file.xhtml?fileId=6561383
[2]:https://dataverse.harvard.edu/file.xhtml?fileId=6565940
[3]:https://dataverse.harvard.edu/file.xhtml?fileId=6561233
