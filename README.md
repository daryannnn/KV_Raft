Key-value хранилище на основе Raft
Новикова Дарья, 20203

## Build

```
cd cmd && go build
```

## Run

```
cd cmd && rm *.dat
./cmd --node 0 --http :2021 --cluster "1,:3030;2,:3031;3,:3032"
./cmd --node 1 --http :2022 --cluster "1,:3030;2,:3031;3,:3032"
./cmd --node 2 --http :2023 --cluster "1,:3030;2,:3031;3,:3032"
```