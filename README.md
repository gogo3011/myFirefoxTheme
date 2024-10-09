# myFirefoxTheme

```
#TabsToolbar {
  visibility: collapse !important;
  display: none !important;
}

#sidebar-header {
  visibility: collapse !important;
} 

#main-window { background-color: #111111 !important; }
/*#323234 for default dark mode theme*/


:root[inFullscreen] #nav-bar{
border-inline: none !important;
}


/* Hide main tabs toolbar */

:root[tabsintitlebar]{
  --uc-window-control-width: 138px; /* Space reserved for window controls */
  //--uc-window-drag-space-width: 24px; /* Extra space reserved on both sides of the nav-bar to be able to drag the window */
}

#nav-bar{
  border-inline: var(--uc-window-drag-space-width,0px) solid transparent;
  border-inline-style: solid !important;
  border-right-width: calc(var(--uc-window-control-width,0px) + var(--uc-window-drag-space-width,0px));
  padding-top: 0px !important;
}



:root{ --uc-toolbar-height: 32px; }

:root:not([uidensity="compact"]){--uc-toolbar-height: 38px}


#TabsToolbar{ visibility: collapse !important }

:root:not([inFullscreen]) #nav-bar{
  margin-top: calc(0px - var(--uc-toolbar-height));
}

#toolbar-menubar{
  min-height:unset !important;
  height:var(--uc-toolbar-height) !important;
  position: relative;
}

#toolbar-menubar:not([inactive]){ z-index: 2 }
#toolbar-menubar[inactive] > #menubar-items {
  opacity: 0;
  pointer-events: none;
  margin-left: var(--uc-window-drag-space-width,0px)
}


```
