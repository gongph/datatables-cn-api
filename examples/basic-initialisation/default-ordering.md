# 缺省排序
使用 DataTables 你可以在初始化的时候修改表格的排序特性。通过使用 `order` 选项来初始化参数配置，用以精准排序你想要的表格数据。

`order` 选项参数是一个二维数组，内部数组的第一个值是指定要排序的列，第二个值是 `asc` （正序）或 `desc` （倒序），它允许多列排序。

下面的 [示例](https://www.datatables.net/examples/basic_init/table_sorting.html) 按年龄进行倒序排序：

Javascript
```js
$(document).ready(function() {
    $('#example').DataTable( {
        "order": [[ 3, "desc" ]] // `Age` 列的索引是 3
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