# 4️⃣ 4. Learn about GitHub Part 2



----------





## Chapter 4 - Project Insights

Features of GitHub for project activity and history

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585845094174_image.png)

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585845120664_Screenshot+from+2020-04-02+12-30-19.png)

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585844998507_image.png)

----------
## Chapter 5 - GitHub General Skills
- Writing in Markdown
- 



## Chapter 6 - Advanced Git Features


- Keeping files out of your projects with `gitignore`
- Hosting your own git repository outside of GitHub
- Adding actions and triggers with the `git` command
- Visualizing project history 
![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585845696812_Screenshot+from+2020-03-23+21-14-30.png)

- View changes from a previous commit
- Git Diff - Show the differences between anything 
    - file vs previous version, 
    - folder vs. other folder
    - folder vs. the same folder yesterday
    - project vs. another project
    - project vs. the same project but different branch




----------



## Chapter 6 - Things to do on GitHub
1. Awesome Lists

Awesome Lists are curated lists of awesome projects found on GitHub and are managed by individual users and communities. There are hundreds of curated lists of awesome projects that you can find on just about any topic.

`https://github.com/onurakpolat/awesome-bigdata`

`https://github.com/academic/awesome-datascience`




## Chapter 7 - GitHub for Non Coding Projects



**Rendering CSV and TSV data**

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585853688441_rendered_csv.png)


When viewed, any *.csv* or *.tsv* file committed to a GitHub repository automatically renders as an interactive table, complete with headers and row numbering. By default, we'll always assume the first row is your header row.
You can link to a particular row by clicking the row number, or select multiple rows by holding down the shift key. Just copy the URL and send it to a friend.
[**Searching data**](https://help.github.com/en/github/managing-files-in-a-repository/rendering-csv-and-tsv-data#searching-data)
If you want to find a certain value in your dataset, you can start typing in the search bar directly above the file. The rows will filter automagically:



**Rendering PDF documents**

GitHub supports rendering of PDF documents.


**Rendering differences in prose documents**

Commits and pull requests that include prose documents have the ability to represent those documents with *source* and *rendered* views.

The source view shows the raw text that has been typed, while the rendered view shows how that text would look once it's rendered on GitHub. For example, this might be the difference between showing `**bold**` in Markdown, and **bold** in the rendered view.

Prose rendering is supported for rendered documents supported by [github/markup](https://github.com/github/markup):

- Markdown
- AsciiDoc
- Textile
- ReStructuredText
- Rdoc
- Org
- Creole
- MediaWiki
- Pod


You can click to see the changes made to the document as part of a commit.

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585853794297_rendered_prose_changes.png)



[**Commenting on changes**](https://help.github.com/en/github/managing-files-in-a-repository/rendering-differences-in-prose-documents#commenting-on-changes)

Commit comments can only be added to files within the *source* view, on a line-by-line basis.

[**Linking to headers**](https://help.github.com/en/github/managing-files-in-a-repository/rendering-differences-in-prose-documents#linking-to-headers)

As with other rendered prose documents, hovering over a header in your document creates a link icon. You can link readers of your rendered prose diff to specific sections.


**Viewing 3D Design Files**

GitHub can host and render 3D files with the *.stl* extension.
When looking directly at an STL file on GitHub you can:

- Click and drag to spin the model.
- Right click and drag to translate the view.
- Scroll to zoom in and out.
- Click the different view modes to change the view.



**Mapping geoJSON files on GitHub**

GitHub supports rendering geoJSON and topoJSON map files within GitHub repositories. Simply commit the file as you would normally using a `.geojson` or `.topojson` extension. Files with a `.json` extension are also supported, but only if `type` is set to `FeatureCollection`, `GeometryCollection`, or `topology`. Then, navigate to the path of the geoJSON file on GitHub.com.
When you click the paper icon on the right, you'll also see the changes made to that file as part of a commit.

Maps on GitHub use [Leaflet.js](http://leafletjs.com/) and support all the geometry types outlined in [the geoJSON spec](http://www.geojson.org/geojson-spec.html) (Point, LineString, Polygon, MultiPoint, MultiLineString, MultiPolygon, and GeometryCollection). TopoJSON files should be type "Topology" and adhere to the [topoJSON spec](https://github.com/mbostock/topojson/wiki/Specification).


**Styling features**

You can customize the way features are displayed, such as specifying a particular color or adding a descriptive icon, by passing additional metadata within the geoJSON object's properties. The options are:

- `marker-size` - `small`, `medium`, or `large`
- `marker-color` - valid RGB hex color
- `marker-symbol` - an icon ID from [the Maki project](http://mapbox.com/maki/) or a single alphanumeric character (a-z or 0-9).
- `stroke` - color of a polygon edge or line (RGB)
- `stroke-opacity` - opacity of a polygon edge or line (0.0 - 1.0)
- `stroke-width` - width of a polygon edge or line
- `fill` - the color of the interior of a polygon (GRB)
- `fill-opacity` - the opacity of the interior of a polygon (0.0-1.0)


**Embedding your map elsewhere**

Want to make your geoJSON map available someplace other than GitHub? Simply modify this template, and place it in any HTML page that supports javascript (e.g., [GitHub Pages](http://pages.github.com/)):


    <script src="https://embed.github.com/view/geojson/<username>/<repo>/<ref>/<path_to_file>"></script>

By default, the embedded map 420px x 620px, but you can customize the output by passing height and width variables as parameters at the end, such as `?height=300&width=500`.



**Working with Jupyter Notebook files on GitHub**

note: A big list of interesting Jupyter Notebooks on GitHub https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks

When you add Jupyter Notebook or IPython Notebook files with a .ipynb extension on GitHub, they will render as static HTML files in your repository.

The interactive features of the notebook, such as custom JavaScript plots, will not work in your repository on GitHub. For an example, see [*Linking and Interactions.ipynb*](https://github.com/bokeh/bokeh-notebooks/blob/master/tutorial/06%20-%20Linking%20and%20Interactions.ipynb).

To view your Jupyter notebook with JavaScript content rendered or to share your notebook files with others you can use [nbviewer](https://nbviewer.jupyter.org/). For an example, see [*Linking and Interactions.ipynb*](https://nbviewer.jupyter.org/github/bokeh/bokeh-notebooks/blob/master/tutorial/06%20-%20Linking%20and%20Interactions.ipynb) rendered on nbviewer.

To view a fully interactive version of your Jupyter Notebook, you can set up a notebook server locally. Or create a GitHub Page for your project with the converted notebook HTML files hosted on GitHub

**Convert the Notebook to HTML**

If you're having trouble rendering Jupyter Notebook files in static HTML, you can convert the file locally on the command line by using the `[nbconvert](https://github.com/jupyter/nbconvert)` [command](https://github.com/jupyter/nbconvert):


    $ jupyter nbconvert --to html NOTEBOOK-NAME.ipynb


Check out the JupyterLab project for more cool things you can do with Jupyter 

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585856341922_jupyterlab.png)

> JupyterLab is the next-generation web-based user interface for Project Jupyter. 

JupyterLab can be extended using [npm](https://www.npmjs.com/) packages that use our public APIs




**Viewing images and image diffs**

GitHub can display several common image formats, including PNG, JPG, GIF, PSD, and SVG. In addition to simply displaying them, there are several ways to compare differences between versions of those image formats.

`https://help.github.com/en/github/managing-files-in-a-repository/rendering-and-diffing-images`

GitHub can display several common image formats, including PNG, JPG, GIF, PSD, and SVG. In addition to simply displaying them, there are several ways to compare differences between versions of those image formats.


- Viewing images
- Viewing differences 
![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585853496467_images-2up-view.png)







**Using GitHub for Design Projects**

![](https://paper-attachments.dropbox.com/s_FE414D50390C26D91A0922774D4358FD54E73D0B0DF25D27D417837C656F72D2_1585846130377_Screenshot+from+2020-04-01+10-16-46.png)


How GitLab’s internal design team uses GitLab for Design Projects 
`https://docs.gitlab.com/ce/user/project/issues/design_management.html`




**Hosting Project Documentation and Team Handbooks** 

    - Project README.md file for every project
    - Project Wiki page
    - Hosting Static HTML Pages directly from your GitHub Project

