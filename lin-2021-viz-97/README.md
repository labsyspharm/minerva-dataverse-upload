# lin-2021-viz-97

## Contact Information

- Principal Investigator: Peter Sorger, Laboratory of Systems Pharmacology, Harvard Medical School (`peter_sorger@hms.harvard.edu`)
- Data Manager: Sarah Arena, Laboratory of Systems Pharmacology, Harvard Medical School (`sarah_arena@hms.harvard.edu`)

## Harvard Dataverse Directory Structure

[Access the full story][full] on the [Harvard Dataverse](https://dataverse.harvard.edu/). The many separate JPEG/PNG files in each Minerva Story have been compressed into additonal ZIP archives for easier management within the Dataverse. Each complete story referenced in this repository can be extracted from the dataverse as follows:

1. First, expand the `dataverse_files.zip` archive.
2. Then, move or copy `lin-2021-viz-97.zip` to `lin-2021-viz-97`.
3. Finally, expand the `lin-2021-viz-97.zip` archive.

The unextracted directories will appear as follows:

```
├── README.md
'── lin-2021-viz-97
  ├── lin-2021-viz-97.zip
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

[full]:https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/BAPIVM
