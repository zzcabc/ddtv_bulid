WORKDIR /DDTVLiveRec
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai' >/etc/timezone
ADD /home/runner/work/ddtv_bulid/ddtv_bulid/ddtv/DDTVLiveRec/bin/Release/net5.0/publish/ /DDTVLiveRec
EXPOSE 11419
VOLUME /DDTVLiveRec/tmp
VOLUME /DDTVLiveRec/BiliUser.ini
VOLUME /DDTVLiveRec/RoomListConfig.json
ENTRYPOINT ["dotnet", "DDTVLiveRec.dll"]
