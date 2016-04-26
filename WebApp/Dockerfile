FROM michaldudak/iis-aspnet

RUN mkdir WebApp

COPY ./WebApp /WebApp
WORKDIR /WebApp

RUN powershell New-WebApplication -Site 'Default Web Site' -ApplicationPool 'DefaultAppPool' -Name 'WebApp' -PhysicalPath 'C:\WebApp'

ENTRYPOINT powershell