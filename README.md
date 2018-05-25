# jQuery selectList
jQuery selectList is a jquery plugin to move selected options from one select box to another. Move single, multiple or all options another select box. Also search and sort content of the options in the select box for easy access.

## Documentation
###Usage
Call selectList() function on any select box group element.
__Example__
	$('#select-list').selectList();

### Options
The plugin accespts following options:

* from (String) - Identifier of the selection list box to select the options from
* to (String) - Identifier of he list box to move the selected list items to
* sort (Boolean) = Sort the list after moving an option (Default true)
* adder (String) - Identifier of the button which on click moves the option to selected list box from available option list box
* remover (String) - Identifier of the button which on click removes the option from selected list box to available option list box
* mover: (String) - Identifier of the button which on click moves all the available options to selected list box from available option list box
* cleaner(String) - Identifier of the button which on click removes all the available options from selected list box to available option list box
* notifier(String) - Class added to the moved option to highlight the option movement activity
* notifytimer (Integer) - Timeout for the notifier class to show in miliseconds (Default: 800)
* fromSearch (String) - Identifier of the search box to search and filter the options in available options list by the content
* toSearch (String) - Identifier of the search box to search and filter the options in selected options list by the content

__Example 1__
	$('#select-list').selectList({
		from: '#fromList',
    to: '#toList',
    sort: true,
    adder: '#add',
    remover: '#remove',
    mover: '#move',
    cleaner: '#clean',
    notifier: 'select-highlight',
    notifytimer: 800,
    fromSearch:'#fromListSearch',
    toSearch:'#toListSearch'
	});
