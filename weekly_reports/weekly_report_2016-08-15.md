# Weekly report

## Week August 8th-15th 2016
Things I did this week:

- submitted issue for scaling issue for images for cyREST (https://github.com/idekerlab/cyREST/issues/46) . Having a hard time getting images from cyREST in an automated fashion that look good. A different issue I am having with RCy3 is that the png and svg images are often cut-off. Will e-mail Tanja about this. 

- completed Tara Oceans vignette: draft available here:https://github.com/jooolia/gsoc_Rcy3_vignettes/blob/master/tara_oceans_co-occurence_net_RCy3_vignette.md
    - incorporated a subnetwork function that could be pulled out for integration into RCy3
  
- draft of paxtoolsr vignette: https://github.com/jooolia/gsoc_Rcy3_vignettes/blob/master/paxtoolsR_vignette.md

- unstuck with clustermaker2, successfully get group information. Now need to see how to work with data that is stored in the network table rather than as a edge or node attribute. 

## Next week: 

For final work product submission:

- Either: 
    - Create a web page or blog post that describes the work you've done and links to the commits you've made. If there is still work to be done on the project, include that too.
    - send a message out to the cytoscape mailing list. send to mentor ahead of time. 
    - If using Github, link to a list of the commits you made: https://github.com/jooolia/gsoc_Rcy3_vignettes/commits/master?author=jooolia , but also https://github.com/tmuetze/Bioconductor_RCy3_the_new_RCytoscape/commits/master?author=jooolia

Get basic steps done on the following vignettes:

- clusterMaker
    - quickly check to see if it is straightforward to work with info in the network table (almost feel it would be easier to run the clustering R and add as an attribute without using clustermaker2). Should
    - can you tell me the cluster that the node is in?
- chemviz
   - create similarity network "chemviz create similarity" a similarity network from a set of nodes
   - installed rcellminer
   - use data pulled from rcellminer 
   - pull out the ones with moa 
   - send to cytoscape
   - create similarity network
   - can put 2D structures on the nodes
   - send the moa info and colour nodes by moa classes. (??) (could take 10 MOAs )
- enrichmentmap
    - will revisit the autoAnnotate 
    - will complete what I have and manually export wordcloud generated. 
    - wrap up what is working
- cyanimator (end)
- make a plan for blog posts that will come out in September
    - one for each vignettes
    - one for experience dealing with the plugins 
         - are they documented, interactions,
         -"in the blog post on using cytoscape plugins (not the individual plugin vignettes) from R please take screenshots of things like what you showed me with the help menu for finding that chemviz could do a similarity network"
         - "… also a description of what you were doing with chrome"
    - experience with cyREST -could also be a good spot to list all the different projects
         - when things were not working how did it go?


## Mentor feedback
- png can be made to be a greater height but not the others.  http://localhost:1234/v1/networks/9632/views/first.png?h=2000 
- made a new function for 
- make note that the images will take on the shape of the window in cytoscape.
- does RCy3 have something for fitting the network to the window? Or maybe just make sure to layout the window before before taking the image?
- could wrap the fit network to the window: http://idekerlab.github.io/cyREST/#-1608791223 is this already in RCy3? yes already in RCy3: `fitContent()`

  
