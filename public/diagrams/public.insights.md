# public.insights

## Description

## Columns

| Name        | Type                        | Default | Nullable | Children                                            | Parents | Comment |
| ----------- | --------------------------- | ------- | -------- | --------------------------------------------------- | ------- | ------- |
| id          | bigint                      |         | false    | [public.insight_members](public.insight_members.md) |         |         |
| user_id     | bigint                      |         | false    |                                                     |         |         |
| name        | varchar                     |         | false    |                                                     |         |         |
| is_public   | boolean                     | false   | true     |                                                     |         |         |
| is_favorite | boolean                     | false   | true     |                                                     |         |         |
| short_code  | varchar                     |         | true     |                                                     |         |         |
| created_at  | timestamp with time zone    | now()   | true     |                                                     |         |         |
| updated_at  | timestamp with time zone    | now()   | true     |                                                     |         |         |
| deleted_at  | timestamp without time zone |         | true     |                                                     |         |         |
| is_featured | boolean                     | false   | false    |                                                     |         |         |

## Constraints

| Name          | Type        | Definition       |
| ------------- | ----------- | ---------------- |
| insights_pkey | PRIMARY KEY | PRIMARY KEY (id) |

## Indexes

| Name          | Definition                                                            |
| ------------- | --------------------------------------------------------------------- |
| insights_pkey | CREATE UNIQUE INDEX insights_pkey ON public.insights USING btree (id) |

## Relations

![er](public.insights.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
