# WhereUsedBookmarks

In the bookmark sidebar, bookmarks search results are provided as a list
with no information about its location in the tree,
despite it is likely usefull to access siblings of bookmarks founds.

I see several possible implementations:

    * unfold result with all parent folders, then show all childs on folder selection
    * unfold path and show siblings on specific right-click context menu "whereUsed"
    * reload the full bookmark view, still selecting the bookmark from witch the context "whereUsed" menu was clicked on.
    * put the folder-path as link to parent folder as an additional properties information.

# Context menu: Where Used

1: Adding context menu on bookmark sidebar (on search-results)
2: show list of parent folder inverted path
2: Open sidebar tree on selected parent folder

1: Adding context menu on bookmark sidebar (on search-results)
https://bugzilla.mozilla.org/show_bug.cgi?id=1370499
https://stackoverflow.com/questions/44118274/add-context-menu-in-bookmark-menu

https://developer.mozilla.org/en-US/Add-ons/WebExtensions/API/menus/ContextType :
Bookmark
Applies when the user context-clicks a bookmark item in the bookmarks toolbar or menu. 
This doesn't currently work for bookmark sidebar and library window items. 
Requires the "bookmarks" API permission in the manifest

Waring menu number has a limit: menus.ACTION_MENU_TOP_LEVEL_LIMIT

2: Showing list of parent folder inverted path
link to parent: 




