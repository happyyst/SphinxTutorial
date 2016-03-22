.. _label_code_block:

代码高亮
============


python 代码
------
.. code-block:: python
    :linenos:

    import random
    def quick_sort(array, left, right):
        if left < right:
            l = left
            r = right
            base = array[l]
            while l < r:
                while l < r and array[r] >= base:
                    r -= 1
                array[l] = array[r]
                while l < r and array[l] < base:
                    l += 1
                array[r] = array[l]
            array[l] = base
            quick_sort(array, left, l - 1)
            quick_sort(array, l + 1, right)


代码行高亮
------
.. code-block:: python
   :emphasize-lines: 3,5
   :linenos:

   def some_function():
       interesting = False
       print 'This line is highlighted.'
       print 'This one is not...'
       print '...but this one is.'

java代码
-------
.. code-block:: java

    public static <E extends Comparable<E>> int binarySearch(E[] array, int from, int to, E key) throws Exception {
        if (from < 0 || to < 0) {
            throw new IllegalArgumentException("params from & length must larger than 0 .");
        }
        if (from <= to) {
            int middle = (from >>> 1) + (to >>> 1); // 右移即除2
            E temp = array[middle];
            if (temp.compareTo(key) > 0) {
                to = middle - 1;
            } else if (temp.compareTo(key) < 0) {
                from = middle + 1;
            } else {
                return middle;
            }
        }
        return binarySearch(array, from, to, key);
    }

html代码
-------

.. code-block:: html

    <body class="">
    <div id="blk_router">
        <div class="loading triangle">
            <div class="loading-mask"></div>
            <div class="loading-indicator"></div>
            <div class="loading-message">
                <p>Please wait while we load an obnoxious amount of JavaScript.</p>
                <p>
                    <small>You may need to disable adblocking extensions to load Sentry.</small>
                </p>
            </div>
        </div>
    </div>
    <script>
        $(function () {
            ReactDOM.render(
                    React.createElement(Router.Router, {history: Sentry.createHistory()}, Sentry.routes),
                    document.getElementById('blk_router')
            );
        });
    </script>
    </body>

