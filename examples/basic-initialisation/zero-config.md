# 零配置
DataTable 默认情况下启用了大部分功能，所以你只需要使用自己的表就可以调用构造函数 `$().DataTable()`。

搜索，排序和分页功能将立即添加到表中，如本[示例](https://www.datatables.net/examples/basic_init/zero_configuration.html)所示。

Javascript
```js
$(document).ready(function() {
    $('#example').DataTable();
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