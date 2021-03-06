#viewer.client-view.and.data.api-Fullstack 

The MIT License (MIT)

Copyright (c) 2014 Autodesk, Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


##Description

*This sample is part of the [Developer-Autodesk/Autodesk-View-and-Data-API-Samples](https://github.com/Developer-Autodesk/autodesk-view-and-data-api-samples) repository.*

A fullstack viewer client sample demonstrating the usage of search, zoom, rotate, model tree, isolate, select, hide API, and etc.

This has a simple htm file, which host the viewer. The htm file has text fields where you need to provide the token and the file urn. 


This sample shows the use of below API’s

      1.Creation of “GuiViewer3D” class.
      
      2.Disabling the property grid in viewer (viewer3D.propertygrid.openOnSelect = false;)
      
      3.Adding camera event callback (viewer3D.addEventListener(Autodesk.Viewing.CAMERA_CHANGE_EVENT, cameraChangedEventCB);
      
      4.Loading the document (Autodesk.Viewing.Document.load())
      
      5.Loading the geometry to show in viewer (viewer3D.load(item3d);)
      
      6.Getting the node from the dbid (viewer3D.model.getNodeById(dbId);)
      
      7.Get the model structure (viewer3D.getObjectTree(getObjectTreeCB);)
      
      8.Isolate the selected geometry using its dbid (viewer3D.isolateById(selectedObjectdbId);)
      
      9.Select the geometry using its dbid (viewer3D.select(selectedObjectdbId);)
      
      10.Hide the geometry using its node (viewer3D.hide(currNode);)
      
      11.Getting geometry properties using dbid (viewer3D.getProperties(selectedObjectdbId, getPropertiesCB);) 
      
      12.Controlling the visibility ghost objects (viewer3D.setGhosting()) 
      
      13.Exploding the geometry between 0 to 1(viewer3D.explode(newVal);)
      
      14.Searching the view for a given text (viewer3D.search(Search, onSearchResultsReturned);)
      
      15.Rotating and zooming of the model (viewer3D.impl.controls.autoMove(automoveType, true);)
      
      16.Event handling of selection, escape, hiding, isolation, camera position changing etc. 

Note: You need to host this htm page in a server. Example: in an ASP.net project or you can use technologies like mongoose etc. 

##Dependencies

The token and file urn can ViewerHelperApp - .NET form based App which can create token, upload files and translate files. This sample give back the urn.

##Setup/Usage Instructions

* Get your consumer key and secret key from http://developer.autodesk.com

You can also watch ViewerDeveloperSample_working.mp4. This shows basic working of the sample.


##Written by 

Virupaksha Aithal


