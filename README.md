# AMI-Widget2 (In development)


AMI-Widget2 is a Polymer 2 application to add widgets easily to your AMI Polymer Application.



# How to use
You should use the Polymer 2 versions of AMI-viewer and AMI-loader (they are provided in the example). The code should be:

```sh
<ami-loader2 
    files="[[files]]" 
    urls="[[urls]]" 
    series="{{series}}">
</ami-loader2>
<ami-viewer2
      series="{{series}}" 
      stackhelper={{stackhelper}} 
      stack={{stack}}
      controls={{controls}} 
      camera={{camera}} 
      threed={{threed}} 
      scene={{scene}} 
      renderer={{renderer}}>
</ami-viewer2>
<ami-widget2 
      stackhelper=[[stackhelper]]
      stack={{stack}} 
      controls={{controls}} 
      camera={{camera}} 
      threed={{threed}} 
      scene={{scene}} 
      renderer={{renderer}}
      guiobjects={{guiobjects}}>
</ami-widget2>
```

Every time you click on your container, AMI-Widget2 will evaluate the `guiobjects` attribute to create the desired widget. You can use `ruler`, `handle`, `annotation`,... The widgets provided in AMI (https://github.com/FNNDSC/ami).
