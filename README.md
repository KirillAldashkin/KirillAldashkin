<h3 align="center">🦊 Приветствую 🦊</h3>
<small>Обычный школьник из России, программист-самоучка.</small>
<h4 align="center">Своё:</h4>
<a href="https://github.com/KirillAldashkin/KiDev.Baikal"><tt>KiDev.Baikal</tt></a>
<div>Библиотека для краткого описания .NET проектов</div>
<pre lang="fs">
#r "nuget: KiDev.Baikal"
open KiDev.Baikal
Solution(__SOURCE_DIRECTORY__)
  |> AddProject(FS()
    |> OutputType Exe
    |> Compile [ Include "Program.fs" ])
  |> run
</pre>

----

<a href="https://github.com/KirillAldashkin/TTFViewer"><tt>TTFViewer</tt></a>
<div>Просмотр TTF шрифтов. Проходится по всем глифам и показывает их контуры.</div>

----

<a href="https://github.com/KirillAldashkin/FindViewByIdCodeGen"><tt>KiDev.FindViewByIdCodegen</tt></a>
<div>Кодогенератор для автоматической привязки элементов в Android Activity</div>
<pre lang="cs">
[SetView(Layout.activity_main)]
public partial class MainActivity : Activity
{
    [FindById(Id.in_elem)] EditText textInput;
    [FindById(Id.out_elem)] TextView textOutput;
    // Метод OnCreate(Bundle) сгенерируется автоматически и привяжет 
    // всё необходимое, после чего будет вызван метод AfterOnCreate() 
    void AfterOnCreate() => textInput.TextChanged += (_, _) => textOutput.Text = textOutput.Text;
}
</pre>
