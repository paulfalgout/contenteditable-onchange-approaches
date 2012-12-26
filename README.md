#Mutation observers vs key events

This snippet is designed to compare the behavior of [mutation observers](https://developer.mozilla.org/en-US/docs/DOM/MutationObserver), using the [mutation summary library](http://code.google.com/p/mutation-summary/), to the variety of key events needed to handle contenteditable changes without mutation events.

Ideas to test out:

1. Quickly run your hand across the numeric keys at the top of your keyboard

	Which approach reports each key individually (should appear as a clean waterfall)?
2. Any differences when copy/pasting?  What about keyboard shortcuts vs context menu?  How about the browser paste button?

	The browser paste button is well-handled by one approach and not at all by the other.  Also, try copying some text, refreshing to start over, and then pasting using the context menu.
3. What about cutting/pasting?

	Try with keyboard shortcuts, the context menu, and the browser buttons.</p>
4. Try highlighting some text in this paragraph and dragging/dropping onto the content editable.