---
layout: doc
title: Sử dụng Geofabrik và HOT Export
permalink: /vi/osm-data/geofabrik-and-hot-export/
lang: vi
category: osm-data
---

Sử dụng Geofabrik và HOT Export
================

> Hướng dẫn này có thể được tải xuống tại đây: [Geofabrik_and_HOT_Export_vi.odt](/files/Geofabrik_and_HOT_Export_vi.odt) or [Geofabrik_and_HOT_Export_vi.pdf](/files/Geofabrik_and_HOT_Export_vi.pdf)  
> Cập nhật: 2017-10-31  

Sau khi học cách thêm và chỉnh sửa dữ liệu trong OpenStreetMap (OSM), bây giờ có thể bạn muốn lấy dữ liệu làm bản sao lưu hoặc xử lý nó bằng phần mềm Hệ thống Thông tin Địa lý mã nguồn mở, chẳng hạn như Quantum GIS ([www.qgis. org] (http://www.qgis.org)).  

TẢI DỮ LIỆU OSM TỪ TRANG WEB GEOFABRIK
-------------------------------------

Các dữ liệu OSM có thể dễ dàng thu được bằng cách tải nó từ [http://download.geofabrik.de/openstreetmap/](http://download.geofabrik.de/openstreetmap/)

[Tải dữ liệu từ geofabrik][]

Dữ liệu được chia thành nhiều vùng. Indonesia có thể được tìm thấy như là một phần của châu Á bằng cách nhấp vào Tiểu khu vực châu Á trên bảng màu xanh và sau đó trang sẽ xuất hiện như thế này.  

![Dữ liệu trên geofabrik của châu Á][]

Sau khi xuất hiện ở đầu trang, xem tiểu vùng chia thành các quốc gia Châu Á như thế nào. Để có được dữ liệu, bạn cần phải nhấp vào nhà nước Indonesia trên bảng màu xanh, và nó sẽ xuất hiện như thế này.  

![Dữ liệu trên geofabrik của Indonesia][]

Sau đó, nếu bạn muốn lấy dữ liệu của Indonesia ở định dạng shapefile (.shp), bạn nhấp vào liên kết indonesia-latest.shp.zip và tệp sẽ được tải xuống. Có một số định dạng có thể được tải xuống. Một định dạng phổ biến là shapefile (shp) với các điểm, polyline, và lớp đa giác.  

Bạn có thể kiểm tra dữ liệu thời gian qua đã được cập nhật. Xin lưu ý, máy chủ thường cập nhật dữ liệu 24 giờ một lần, vì vậy nếu bạn chỉ cần tải dữ liệu lên OSM thì dữ liệu sẽ không xuất hiện tự động khi bạn tải xuống, nhưng bạn phải đợi các cập nhật mới nhất từ máy chủ.  

Tải dữ liệu OSM từ công cụ trích xuất dữ liệu HOT
--------------------------------------

Nhóm [Humanitarian OpenStreetMap Team] (https://www.hotosm.org) đã tạo ra một dịch vụ trực tuyến cho phép người dùng tạo ra các trích xuất dữ liệu OSM tuỳ chỉnh bất cứ nơi nào trên thế giới, bằng cách chọn một khu vực quan tâm, các loại đối tượng bản đồ và định dạng tệp tin. Dịch vụ có tại [export.hotosm.org] (https://export.hotosm.org/en/v3). Trong vòng vài phút, dữ liệu OpenStreetMap cập nhật (OSM) được xuất, lọc và chuyển đổi.  Phần tiếp theo sẽ hướng dẫn bạn cách thức sử dụng công cụ trích xuất dữ liệu. Các thông tin này cũng có thể tìm thấy trong mục '[Tìm hiểu] (https://export.hotosm.org/en/v3/learn)' tại export.hotosm.org.

![hot-export-tool][]

## Bắt đầu

Bất cứ ai cũng có thể tạo một tùy chỉnh xuất dữ liệu OpenStreetMap với Export Tool - chỉ cần đăng ký một tài khoản. Bạn có thể đăng ký với một tài khoản OpenStreetMap từ openstreetmap.org, và một địa chỉ email hợp lệ, sẽ được sử dụng để gửi một liên kết đến phiên trích xuất dữ liệu của bạn sau khi hoàn tất.

## Lựa chọn vùng xuất dữ liệu - Area of Interest

Có nhiều cách để lựa chọn vùng xuất dữ liệu (AOI) thông qua Công cụ Trích xuất. Điều này bao gồm khả năng nhập và tìm kiếm, xác định các tọa độ của một hộp bao quanh, vẽ một hộp bao quanh, vẽ một đa giác, dùng khung nhìn hiện tại hoặc tải tệp tin địa lý geojson lên.

![export-tool-create][]

Khi bạn đã 'Đăng nhập' vào Công cụ xuất dữ liệu HOT, tab 'Tạo' sẽ được kích hoạt. Tab 'Tạo' là nơi bạn sẽ thiết lập các tùy chọn cho việc xuất dữ liệu, bằng cách mô tả nó ở phía bên tay trái và chọn vùng xuất dữ liệu với bản đồ ở phía bên tay phải. 

![export-tool-describe][]

### Thanh công cụ tìm kiếm
Có 6 cách để xác định cùng xuất dữ liệu của bạn. Cách thứ nhất và thứ hai là sử dụng thanh tìm kiếm, nơi có thể tìm địa điểm bằng cách nhập tên và chọn nó từ các tùy chọn bên dưới hoặc bằng cách xác định tọa độ của vùng bao. Bạn có thể tìm thấy tọa độ X cực đại, X cực tiểu, Y cực đại và Y cực tiểu (Tây, Nam, Đông, Bắc) của một quốc gia [trong một danh sách CSV do Cơ quan trao đổi dữ liệu nhân đạo (Humanitarian Data Exchange - HDX) cung cấp (https://data.humdata.org/dataset/bounding-boxes-for-countries).

![export-tool-search][]
![export-tool-coordinates][]


### Số hóa 
Cách thứ ba và thứ tư để chọn vùng xuất dữ liệu trong Export Tool là bằng cách vẽ một hộp bao quanh bằng tùy chọn 'Box' từ cột công cụ ở bên phải của màn hình. Hoặc bạn có thể tự do vẽ đa giác trực tiếp trên bản đồ bằng cách chọn công cụ 'Vẽ'.

![export-tool-area-bbox][]
![export-tool-area-draw][]


### Tải lên vùng xuất dữ liệu
Hai cách cuối cùng để chọn vùng xuất dữ liệu là thông qua chọn 'Vùng hiển thị' ở phía bên tay phải của bản đồ, để sử dụng phạm vi của chế độ xem hiện tại của bản đồ hoặc bằng công cụ 'Nhập' cho phép bạn tải lên một đa giác của vùng lựa chọn.  

![export-tool-area-view][]
![export-tool-area-import1][]


The imported polygon must be a GeoJSON file in WGS84 geographic coordinates. One of the ways to create a GeoJSON file is to use the geojson.io site. Once the area has been selected in [geojson.io](http://geojson.io/), copy the text in the box to the right, paste it into an editor of choice, such as [Atom](https://atom.io/) and save your GeoJSON file.

![export-tool-geojson-io][]
![export-tool-geojson-edit1][]


The GeoJSON file needs to be edited slightly in order for it to be accepted by the Export Tool. Please note that the file can not be multipolygons. In the simplest form the file only needs to state that it is a “type: Polygon” and list the coordinates of the points/nodes that identify the area. The GeoJSON file will then successfully be parsed by the tool and used to specify the AOI.

![export-tool-geojson-edit2][]
![export-tool-area-import2][]


## Select File Formats

The tool allows OSM data to be extracted through the Overpass API in its native Protocol Buffer Binary (PBF) file format, before filtering the data for the map features and associated tags specified by the user. Once the data has been filtered it is then converted into the file formats chosen by the user.  

Currently the tool can convert OSM data into Shapefile .shp, GeoPackage .gpkg, Garmin .img, Google Earth .kml, OSM .pbf, MAPS.ME .mwm, OsmAnd .obf, and MBTiles .mbtiles. At least one of the file formats must be selected to create the export, but there is no restriction as to how many can be chosen, which can be done by ticking multiple boxes.

![export-tool-file-formats][]


### Shapefile .shp
Shapefiles are a tabular format developed by Esri. They are the most popular file format for GIS data. A shapefile is actually 3-4 individual files, commonly bundled together as a ZIP archive. Shapefiles do have certain limitations, such as the file size, capping at 2 gigabytes (GB) and a column name length limit of 10 characters. Read more about [Shapefiles .shp](https://export.hotosm.org/en/v3/learn/export_formats#shp) in the Learn section.

![export-tool-shapefile][]


### Geopackage .gpkg
OGC Geopackages store geospatial data in a single SQLite database. Geopackages are very similar to Spatialite-enabled SQLite databases. They should be usable in most major GIS applications. Geopackages support practically unlimited file sizes and numbers of columns in tables, and have full support for Unicode. They are especially ideal if you need to run SQL queries over the data. Read more about [Geopackages.gpkg](https://export.hotosm.org/en/v3/learn/export_formats#gkpg) in the Learn section.

![export-tool-sql][]


### Garmin .img
A .IMG file contains all information needed to render a map onto a Garmin GPS mobile device. Please note that the cartographic .img style and feature choices of the map are not dependent on the feature selection submitted to the Export Tool - instead, a default style based on all OSM data is used. Read more about [Garmin .img](https://export.hotosm.org/en/v3/learn/export_formats#img) in the Learn section.

![export-tool-garmin][]


### Google Earth .kml
The Keyhole Markup Language (KML) is an XML-based format for modeling points, lines, polygons and associated attributes geographically. Google Earth is the most widely known earth view browsing platform using KML, which is also the reason why it was developed. Read more about [Google Earth .kml](https://export.hotosm.org/en/v3/learn/export_formats#kml) in the Learn section.

![export-tool-google-earth][]


### OSM .pbf
The canonical data format of OSM is an XML document of nodes, ways and relations. The Protocol Buffer Binary Format (PBF) is an optimised representation of OSM XML, which is smaller on disk and faster to read. This format is only compatible with OSM specific tools, such as OSM editing software. Each .PBF provided by the export tool should be referentially complete - that is, any node, way or relation referenced by a way or relation will appear in the PBF. Learn more about [OSM .pbf](https://export.hotosm.org/en/v3/learn/export_formats#pbf) in the Learn section.

![export-tool-xml-code][]


### MAPS.ME .mwm
Maps.me is a GPS Navigation and map application for Android and iOS smartphones and tablets, notably supporting offline mapping and navigation. Read more about [MAPS.ME .mwm](https://export.hotosm.org/en/v3/learn/export_formats#mwm) in the Learn section. To use a custom export with Maps.me on Android, please follow these steps:
Open Maps.me and navigate to your region of interest
Accept Maps.me's prompt and download the offered region
Force close Maps.me
Create an MWM export
Download the export, unzip it, and copy the .mwm file to your device
Using the Android File Manager, navigate to the location containing the .mwm file
Long-press to select it and touch the "copy" or "cut" button
Navigate to "MapsWithMe" and open the highest numbered folder (e.g. 170917)
Copy/move your .mwm file into this directory by tapping the "paste" button
Delete the existing .mwm file for your region of interest, taking note of its filename
Rename your .mwm file to match the region that was downloaded by Maps.me (which you just deleted) by long-pressing (to select) and tapping the "more" button (3 vertical dots)
Open Maps.me

![export-tool-mapsme][]


### OsmAnd .obf
OsmAnd is also a GPS Navigation and map application for Android and iOS smartphones, as well as  tablets, notably supporting offline rendering, routing, and searching. Read more about the application and its numerous features of [OsmAnd .obf](https://export.hotosm.org/en/v3/learn/export_formats#obf) from their main website. 

![export-tool-osmand][]


### MBTiles .mbtiles
MBTiles is a file format for storing map tiles in a single file. The Export Tool allows users to create MBTiles containing tiles from OSM, which can be used as sources of offline context within applications that support them. Please note that MBTiles will extract all the OSM features in the selected area of interest through the Export Tool, with the ‘3 Data’ tab automatically switching to a dropdown source option and zoom range, in place of the standard tree tag and YAML feature selection option. Read more about [MBTiles .mbtiles](https://export.hotosm.org/en/v3/learn/export_formats#mbtiles) in the Learn section.

![export-tool-mbtiles][]


Additional file formats are continuously being suggested and added to the Export Tool. If there is a file format that you would like to see added in the future, please make a comment on the [GitHub](https://github.com/hotosm/osm-export-tool/issues) repository. For further detailed information regarding each file format type, please visit the ‘File Formats’ page in the ‘[Learn](https://export.hotosm.org/en/v3/learn)’ section on the tool website.



## Customise Map Features

The tool allows the user to customise the data selected within the defined area of interest. The OSM data is defined by using tag filters and key selections, with the Tag Tree or YAML Form. The Tag Tree is for common use cases, presenting a curated set of filters and selections, where the YAML configuration provides complete control over filters and selections, using a SQL-like filter definition.

![export-tool-treetag-tab][]
![export-tool-yaml-tab][]


OSM is an open global database of tagged geographic features, with three types of elements:
Nodes, which represent a point on the surface of the earth
Ways, which are sets of nodes that can form lines or polygons
Relations, which are sets of nodes, ways or other relations

Each of these elements can have any number of key=value tags. For example, a post office may be represented by a way with the tags building=yes and amenity=post_office. Lets see how these tags can be defined in the Export Tool using the Tag Tree and YAML Form to filter OSM data.

### Tag Tree
The Tag Tree is the simplest way to get started selecting features, simply by ticking the desired parent or child checkboxes. Please note that selecting a parent checkbox will add additional key=value tags associated to the theme, as well as the child checkboxes below it. Each parent checkbox has a different query to filter data, so it is highly recommended that the syntax for each theme is explored by hovering over the checkbox, which will provide an info box to the right. 

![export-tool-treetag-sql][]


For example selecting the ‘Emergency’ parent checkbox, will automatically select the ‘Police Station’, ‘Ambulance Station’ and ‘Fire Station’ child checkboxes below it, yet in addition to this it will also select all tags where emergency=yes, amenity=police and amenity=fire_station in the following SQL query:

emergency IS NOT NULL OR amenity IN ('police','fire_station')

The parent checkboxes do not always represent what is available as children below, to try and account for all possible tags associated with a theme. OSM tags are continuously evolving and we want to ensure that the tool can adapt to these changes. Only the most commonly used key=value tags are represented as child checkboxes, and the parent checkboxes are used to try and encompass those not used as frequently, but fall within a theme. If you have suggestions for modifications to these themes and tags, please comment on the [spreadsheet](https://docs.google.com/spreadsheets/d/10e9HrMkAiy0zyLj1l_mfNsAPp0P4Yyh6W7JvnZx6BBA/edit#gid=0) used to populate the Tag Tree, and we will try to incorporate it where appropriate.

![export-tool-treetag-spreadsheet][]


### YAML Form
Using a YAML configuration provides complete control over applying filters to the OSM data, by using a SQL-like filter definition to apply key=value tags. Please note that the Tag Tree also generates syntax on the YAML Form, so any parent and child checkboxes selected will automatically be applied in the YAML box. This acts as a starting point for the query which can be further edited. 

![export-tool-treetag-yaml][]


The use of YAML was chosen due to its simplicity and compatibility with SQL. The YAML feature selection format  is similar to style files used by programs such as osm2pgsql and imposm. It is whitespace sensitive, with each child element indented below its parent element, and preceded by a dash. This dash must have a space after it. Here is a basic example of a feature selection with 3 themes, buildings, waterways and hospitals:

![export-tool-yaml-code1][]


YAML has Themes, and two data structures, Mapping and Lists
Theme in the above example is: buildings
Mappings in the above example are: types and select 
Lists in the above example are: child elements of select and types

YAML: Themes
Themes are the top level keys in the YAML document, with valid characters including letters, numbers and underscores. 

YAML: Geometry Types
The list values under the mapping types can be one or more of ‘- points’, ‘- lines’, ‘- polygons’. If the types key is omitted, all three geometry types will be included in the theme.

YAML: Column Selections
List items under the mapping select key determines the columns for each theme. The following example will populate the ‘name’ and ‘amenity’ columns with their values from OSM:

![export-tool-yaml-code2][]


YAML: Filters
Filters are under the where: key in each theme. They define what subset of OSM features belongs to that theme. The following example will filter the theme to only features where the key natural has the value waterway:

![export-tool-yaml-code3][]


Please note It is almost always necessary to have some kind of filtering, otherwise the theme will simply include all OSM features for the given geometry types. A filter is specified using SQL-like syntax, with valid keywords IS NOT NULL, AND, OR, IN, =, !=.

![export-tool-yaml-code4][]


JOSM Presets
Older versions of the Export Tool used JOSM Preset .XML files to define feature selections. The new version uses YAML as it is more flexible in how it transforms OSM data. The new Export Tool, however can help convert JOSM presets into YAML configurations, by selecting the ‘Load from JOSM Preset .XML’ button. Please note If the preset is more complex, it may need to be written as a new YAML configuration based on the ‘item’ elements contained in the XML.

![export-tool-load-preset][]



### Configurations

YAML configurations can be defined and saved for future use through the ‘Configs’ page. It's useful to create one configuration for a project, which can then used on all exports related to that project. Give the configuration a ‘name’ and ‘description’ that will make it discoverable by other users. Unchecking the ‘Public’ checkbox will make the configuration visible to only the user. 

![export-tool-configuration-saved][]


Please note that configurations can be edited, which is useful for evolving a feature selection during the course of a project. Saved YAML configurations can be selected via the ‘Stored Configuration’ option on the ‘3 Data’  tab when creating an export. Use the Search bar to find configurations related to your project.

![export-tool-configuration-stored][]


For further detailed information regarding feature selections and YAML, please visit the ‘Selecting Features’ and ‘YAML Specification’ in the ‘[Learn](https://export.hotosm.org/en/v3/learn)’ section on the tool website. 




[Tải dữ liệu từ geofabrik]: /images/osm-data/download-geofabrik.png
[Dữ liệu trên geofabrik của châu Á]: /images/osm-data/geofabrik-asia.png
[Dữ liệu trên geofabrik của Indonesia]: /images/osm-data/geofabrik-indonesia.png
[hot-export-tool]: /images/osm-data/hot-export-tool.png
[export-tool-create]: /images/osm-data/export-tool-create.png
[export-tool-describe]: /images/osm-data/export-tool-describe.png
[export-tool-search]: /images/osm-data/export-tool-search.png
[export-tool-coordinates]: /images/osm-data/export-tool-coordinates.png
[export-tool-area-bbox]: /images/osm-data/export-tool-area-bbox.png
[export-tool-area-draw]: /images/osm-data/export-tool-area-draw.png
[export-tool-area-view]: /images/osm-data/export-tool-area-view.png
[export-tool-area-import1]: /images/osm-data/export-tool-area-import1.png
[export-tool-geojson-io]: /images/osm-data/export-tool-geojson-io.png
[export-tool-geojson-edit1]: /images/osm-data/export-tool-geojson-edit1.png
[export-tool-geojson-edit2]: /images/osm-data/export-tool-geojson-edit2.png
[export-tool-area-import2]: /images/osm-data/export-tool-area-import2.png
[export-tool-file-formats]: /images/osm-data/export-tool-file-formats.png
[export-tool-shapefile]: /images/osm-data/export-tool-shapefile.png
[export-tool-sql]: /images/osm-data/export-tool-sql.png
[export-tool-garmin]: /images/osm-data/export-tool-garmin.jpg
[export-tool-google-earth]: /images/osm-data/export-tool-google-earth.jpg
[export-tool-xml-code]: /images/osm-data/export-tool-xml-code.png
[export-tool-mapsme]: /images/osm-data/export-tool-mapsme.png
[export-tool-osmand]: /images/osm-data/export-tool-osmand.png
[export-tool-mbtiles]: /images/osm-data/export-tool-mbtiles.jpg
[export-tool-treetag-tab]: /images/osm-data/export-tool-treetag-tab.png
[export-tool-yaml-tab]: /images/osm-data/export-tool-yaml-tab.png
[export-tool-treetag-sql]: /images/osm-data/export-tool-treetag-sql.png
[export-tool-treetag-spreadsheet]: /images/osm-data/export-tool-treetag-spreadsheet.png
[export-tool-treetag-yaml]: /images/osm-data/export-tool-treetag-yaml.png
[export-tool-yaml-code1]: /images/osm-data/export-tool-yaml-code1.png
[export-tool-yaml-code2]: /images/osm-data/export-tool-yaml-code2.png
[export-tool-yaml-code3]: /images/osm-data/export-tool-yaml-code3.png
[export-tool-yaml-code4]: /images/osm-data/export-tool-yaml-code4.png
[export-tool-load-preset]: /images/osm-data/export-tool-load-preset.png
[export-tool-configuration-saved]: /images/osm-data/export-tool-configuration-saved.png
[export-tool-configuration-stored]: /images/osm-data/export-tool-configuration-stored.png




