WORKDIR /DDTVLiveRec
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai' >/etc/timezone
ADD ./publish /DDTVLiveRec
EXPOSE 11419
VOLUME /DDTVLiveRec/tmp
VOLUME /DDTVLiveRec/BiliUser.ini
VOLUME /DDTVLiveRec/RoomListConfig.json
ENTRYPOINT ["dotnet", "DDTVLiveRec.dll"]
