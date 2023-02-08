<h6 align="right">Как-то криво тут всё, надо будет доделать</h6>
<h3 align="center">🦊 Приветствую 🦊</h3>
<p>Обычный школьник из России, программист-самоучка.</p>
<h4 align="center">Проекты:</h4>
<img src="https://baikal-safari.com/images/%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D0%B0%D0%BA%D1%82%D0%B8%D0%B2%D0%BD%D0%B0%D1%8F%20%D0%BA%D0%B0%D1%80%D1%82%D0%B0%20%D0%BE%D1%82%D0%B4%D1%8B%D1%85%D0%B0%20%D0%BD%D0%B0%20%D0%B1%D0%B0%D0%B9%D0%BA%D0%B0%D0%BB%D0%B5.png" width="16%" align="left"><a href="https://github.com/KirillAldashkin/KiDev.Baikal"><tt>KiDev.Baikal</tt></a> - библиотека для краткого описания .NET проектов:
<pre lang="fs">
#r "nuget: KiDev.Baikal"
open KiDev.Baikal
Solution(__SOURCE_DIRECTORY__)
  |> AddProject(FS()
    |> OutputType Exe
    |> Compile [ Include "Program.fs" ])
  |> run
</pre>
<br clear="left"/>
