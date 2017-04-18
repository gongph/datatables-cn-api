# 功能启用/禁用
禁用不希望用于特定表的功能很容易通过在初始化对象中设置变量来完成。可以使用的选项的完整列表可在[这里](https://datatables.net/reference/option) 查看。

在本[示例](https://www.datatables.net/examples/basic_init/filter_only.html)中，只有搜索功能保持启用（默认情况下是这样）。

Javascript
```js
$(document).ready(function() {
    $('#example').DataTable( {
        "paging":   false,
        "ordering": false,
        "info":     false
    } );
});
```

HTML
```html 
<table id="example" class="display" cellspacing="0" width="100%">
        <thead>
            <tr>
                <th>Name</th>
                <th>Position</th>
                <th>Office</th>
                <th>Age</th>
                <th>Start date</th>
                <th>Salary</th>
            </tr>
        </thead>
        <tfoot>
            <tr>
                <th>Name</th>
                <th>Position</th>
                <th>Office</th>
                <th>Age</th>
                <th>Start date</th>
                <th>Salary</th>
            </tr>
        </tfoot>
        <tbody>
        	...
        </tbody>
</table>
```