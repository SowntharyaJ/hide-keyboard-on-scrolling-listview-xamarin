# How to hide the keyboard when scrolling in Xamarin.Forms ListView?

This example demonstrate how to hide the keyboard when scrolling in Xamarin.Forms ListView.

## Sample

```xaml
<syncfusion:SfListView x:Name="listView" AutoFitMode="DynamicHeight" ItemsSource="{Binding ContactsInfo}">
<syncfusion:SfListView.ItemTemplate >
    <DataTemplate>
        <Grid x:Name="grid">
            <Grid.ColumnDefinitions>
                <ColumnDefinition Width="70" />
                <ColumnDefinition Width="*" />
            </Grid.ColumnDefinitions>
            <Image Source="{Binding ContactImage}" VerticalOptions="Center" HorizontalOptions="Center" HeightRequest="50" WidthRequest="50"/>
            <Grid Grid.Column="1" RowSpacing="1" Padding="10,0,0,0" VerticalOptions="Center">
                <Label LineBreakMode="NoWrap" TextColor="#474747" Text="{Binding ContactName}" VerticalOptions="Center" FontSize="15"/>
                <Entry Grid.Row="1" Grid.Column="0" TextColor="#474747" Text="{Binding ContactNumber}" VerticalOptions="Center"/>
            </Grid>
        </Grid>
    </DataTemplate>
</syncfusion:SfListView.ItemTemplate>
</syncfusion:SfListView>
```
**[View document in Syncfusion Xamarin Knowledge base](https://www.syncfusion.com/kb/12559/how-to-hide-the-keyboard-when-scrolling-in-xamarin-forms-listview-sflistview)**

## Requirements to run the demo

* [Visual Studio 2017](https://visualstudio.microsoft.com/downloads/) or [Visual Studio for Mac](https://visualstudio.microsoft.com/vs/mac/)
* Xamarin add-ons for Visual Studio (available via the Visual Studio installer).

## Troubleshooting

### Path too long exception

If you are facing path too long exception when building this example project, close Visual Studio and rename the repository to short and build the project.

