# Playlist
Gabriela-INF2B


package com.example.agendiario;

import androidx.annotation.NonNull;
import androidx.annotation.Nullable;
import androidx.room.ColumnInfo;
import androidx.room.Entity;
import androidx.room.PrimaryKey;


@Entity(tableName = "playlist")

class Playlist {

    @PrimaryKey(autoGenerate = true)
    @NonNull
    @ColumnInfo(title = "playlistId")
    private int playlistId;

    @Nullable
    @ColumnInfo(title = "playlistTitle")
    private String playlistTitle;

    private String playlistSinger;

    public Donation(@Nullable String title, String singer, int score, String creationDate) {
        playlistTitle = title;
        playlistSinger = Singer;
        playlistScore = score;
        playlistCreationDate = creationDate;
    }

    public int getId() {
        return playlistId;
    }

    public void setId(int id) {
        playlistId = id;
    }

    public String getTitle() {
        return playlistTitle;
    }

    public void setTitle(String title) {
        playlistTitle = title;
    }

    public String getSinger() {
        return playlistSinger;
    }

    public void setSinger(String singer) {
        playlistSinger = singer;
    }

    public int getScore() {
        return playlistScore;
    }

    public void setScore(int score) {
        playlistScore = score;
    }

    public String getCreationDate() {
        return playlistCreationDate;
    }

    public void setCreationDate(String creationDate) {
        playlistCreationDate = creationDate;
    }

    private int playlistScore;
    private String playlistCreationDate;

}



