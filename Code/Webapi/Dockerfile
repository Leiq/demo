FROM microsoft/aspnetcore:2.0
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
ARG source
WORKDIR /app
EXPOSE 80
COPY ./bin/Release/PublishOutput .
ENTRYPOINT ["dotnet", "Webapi.dll"]
