## Task
  
  1. Реализовать кастомный обработчик запроса - [IHttpHandler](https://docs.microsoft.com/en-us/dotnet/api/system.web.ihttphandler?view=netframework-4.7.2), который возвращает изображение, находящееся в некотором каталоге приложения.
  
  2. Реализовать кастомный обработчик маршрута - [IRouteHandler](https://docs.microsoft.com/en-us/dotnet/api/system.web.routing.iroutehandler?view=netframework-4.7.2), который используется для обработки маршрута c URL-паттерном **Image/{id}** и устанавливает для дальнейшей обработки запроса IHttpHandler из п.1.
  
  Примеры ниже.
   ### ![](https://github.com/AnzhelikaKravchuk/Training-Autumn-2018/blob/master/Pictures/1.png)
    
   ### ![](https://github.com/AnzhelikaKravchuk/Training-Autumn-2018/blob/master/Pictures/2.png)
    
   ### ![](https://github.com/AnzhelikaKravchuk/Training-Autumn-2018/blob/master/Pictures/3.png)
  
  3. *(draft)* Реализовать кастомный управляемый модуль - [IHttpModule](https://docs.microsoft.com/en-us/dotnet/api/system.web.ihttpmodule?view=netframework-4.7.2).
