## How to disable the hover color for the header cell in a Flutter DataTable?

In this article, we will show you how to disable the hover color for the header cell in a [Flutter DataTable](https://www.syncfusion.com/flutter-widgets/flutter-datagrid).

Initialize the [SfDataGrid](https://pub.dev/documentation/syncfusion_flutter_datagrid/latest/datagrid/SfDataGrid-class.html) widget with all the required properties. You can change the appearance of the grid using [SfDataGridThemeData](https://pub.dev/documentation/syncfusion_flutter_core/latest/theme/SfDataGridThemeData-class.html) in the [SfDataGridTheme](https://pub.dev/documentation/syncfusion_flutter_core/latest/theme/SfDataGridTheme-class.html). The DataGrid should be wrapped inside the SfDataGridTheme. To restrict the hover color of header cells, set the header hover color to transparent using [SfDataGridThemeData.headerHoverColor](https://pub.dev/documentation/syncfusion_flutter_core/latest/theme/SfDataGridThemeData/headerHoverColor.html).

```dart
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text('Syncfusion Flutter DataGrid'),
      ),
      body: SfDataGridTheme(
        data: SfDataGridThemeData(headerHoverColor: Colors.transparent),
        child: SfDataGrid( ),
      ),
    );
  }
```

You can download this example on [GitHub](https://github.com/SyncfusionExamples/How-to-disable-the-hover-color-for-the-header-cell-in-a-Flutter-DataTable).