## Data Definition Language (DDL) for server side data model

```sql
create sequence hibernate_sequence start with 1 increment by 1;
create table follow
(
    follower_id bigint not null,
    followed_id bigint not null,
    primary key (follower_id, followed_id)
);
create table history
(
    history_id   bigint not null,
    close_price  float,
    date         date   not null,
    high_price   float,
    low_price    float,
    open_price   float,
    trade_volume bigint,
    stock_id     bigint not null,
    primary key (history_id)
);
create table industry
(
    industry_id bigint       not null,
    name        varchar(255) not null,
    primary key (industry_id)
);
create table preferred
(
    user_id     bigint not null,
    industry_id bigint not null
);
create table stock
(
    stock_id          bigint       not null,
    company           varchar(255) not null,
    fifty_two_wk_high double       not null,
    fifty_two_wk_low  double       not null,
    nasdaq_name       varchar(255) not null,
    plot_path         varchar(255),
    price             double       not null,
    industry_id       bigint,
    primary key (stock_id)
);
create table stock_share
(
    user_id  bigint not null,
    stock_id bigint not null
);
create table user_info
(
    user_id   bigint       not null,
    created   timestamp    not null,
    name      varchar(255) not null,
    oauth_key varchar(255) not null,
    primary key (user_id)
);
alter table user_info
    add constraint UK_f10u70em169ls649ad76e7rhu unique (oauth_key);
alter table follow
    add constraint FKp1n3sm9pih7onqsviuoirh5g2 foreign key (followed_id) references user_info;
alter table follow
    add constraint FK589qlw8jasjl2m22avok2skbm foreign key (follower_id) references user_info;
alter table history
    add constraint FK5ssx6x29m2p8vmv1aeej6d2pn foreign key (stock_id) references stock;
alter table preferred
    add constraint FK9qphu0gtbw59lieo1397hl3np foreign key (industry_id) references industry;
alter table preferred
    add constraint FK22ief5h6gqkf9c6p72s7q5dl foreign key (user_id) references user_info;
alter table stock
    add constraint FKodmbmjf3j49l4bd01lrm6feyw foreign key (industry_id) references industry;
alter table stock_share
    add constraint FK8suvjsnkmqif4ru60o4ow8cvp foreign key (stock_id) references stock;
alter table stock_share
    add constraint FKp1uq9nwylmdtxxujnw64fku2b foreign key (user_id) references user_info;
create sequence hibernate_sequence start with 1 increment by 1;
create table follow
(
    follower_id bigint not null,
    followed_id bigint not null,
    primary key (follower_id, followed_id)
);
create table history
(
    history_id   bigint not null,
    close_price  float,
    date         date   not null,
    high_price   float,
    low_price    float,
    open_price   float,
    trade_volume bigint,
    stock_id     bigint not null,
    primary key (history_id)
);
create table industry
(
    industry_id bigint       not null,
    name        varchar(255) not null,
    primary key (industry_id)
);
create table preferred
(
    user_id     bigint not null,
    industry_id bigint not null
);
create table stock
(
    stock_id          bigint       not null,
    company           varchar(255) not null,
    fifty_two_wk_high double       not null,
    fifty_two_wk_low  double       not null,
    nasdaq_name       varchar(255) not null,
    plot_path         varchar(255),
    price             double       not null,
    industry_id       bigint,
    primary key (stock_id)
);
create table stock_share
(
    user_id  bigint not null,
    stock_id bigint not null
);
create table user_info
(
    user_id   bigint       not null,
    created   timestamp    not null,
    name      varchar(255) not null,
    oauth_key varchar(255) not null,
    primary key (user_id)
);
alter table user_info
    add constraint UK_f10u70em169ls649ad76e7rhu unique (oauth_key);
alter table follow
    add constraint FKp1n3sm9pih7onqsviuoirh5g2 foreign key (followed_id) references user_info;
alter table follow
    add constraint FK589qlw8jasjl2m22avok2skbm foreign key (follower_id) references user_info;
alter table history
    add constraint FK5ssx6x29m2p8vmv1aeej6d2pn foreign key (stock_id) references stock;
alter table preferred
    add constraint FK9qphu0gtbw59lieo1397hl3np foreign key (industry_id) references industry;
alter table preferred
    add constraint FK22ief5h6gqkf9c6p72s7q5dl foreign key (user_id) references user_info;
alter table stock
    add constraint FKodmbmjf3j49l4bd01lrm6feyw foreign key (industry_id) references industry;
alter table stock_share
    add constraint FK8suvjsnkmqif4ru60o4ow8cvp foreign key (stock_id) references stock;
alter table stock_share
    add constraint FKp1uq9nwylmdtxxujnw64fku2b foreign key (user_id) references user_info;
```

[`ddl.sql`](ddl.sql)