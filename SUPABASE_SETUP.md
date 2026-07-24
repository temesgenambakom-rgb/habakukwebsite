# Supabase Database Qopheessuu - Tartiiba

## 1. Supabase irratti Database Uumuu

1. **supabase.com** deemi, account bilisaa (free) banadhu (GitHub'iin sign in godhuu ni dandeessa)
2. **New Project** cuqaasi
3. Maqaa project (fkn `habakuk-students`) galchi
4. **Database Password** cimaa uumi — **kaa'i, ni barbaachisa!**
5. Region (naannoo server) filadhu — kan biyya keessan waliin dhihoo ta'e
6. **Create new project** cuqaasi (daqiiqaa 1-2 fudhata)

## 2. Connection String (DATABASE_URL) Argachuu

1. Project kee keessa, **Settings** (gear icon) → **Database** cuqaasi
2. Kutaa **Connection String** jalatti, tab **URI** filadhu
3. Link akka kanaa argatta:
   ```
   postgresql://postgres.xxxxx:[YOUR-PASSWORD]@aws-0-xxxxx.pooler.supabase.com:6543/postgres
   ```
4. `[YOUR-PASSWORD]` bakka buusi password Step 1 irratti uumte sanaan

## 3. Render Environment Variables keessatti Galchuu

Render dashboard, Web Service kee keessa:

1. **Environment** tab cuqaasi
2. **Add Environment Variable** cuqaasii kanneen galchi:
   - `DATABASE_URL` = connection string Step 2 irraa argatte
   - `SECRET_KEY` = jecha dheeraa fi cimaa (fkn random characters)
   - `ADMIN_USERNAME` = maqaa admin barbaaddu
   - `ADMIN_PASSWORD` = password admin cimaa
3. **Save Changes** cuqaasi — app-ni ofumaan deploy irra deebi'a

## 4. Mirkaneessuu (Verify)

App-ni erga deploy xumuramee booda, link kee bani. Yoo login/register milkaa'e, database-ni Supabase waliin walqunnamee jira jechuudha.

Supabase Dashboard → **Table Editor** keessatti tables `students` fi `school_accounts` argita.

## Xiyyeeffannaa

- Password Supabase kee eessumaayyuu hin ibsin (kan si qofa beeku)
- Waggaa tokkoof yoo fayyadamtan (schools guyyaa guyyaan seenan), project-ni "pause" hin ta'u
- Kanaan ala backup Excel (ji'a ji'aan) fayyadamuun itti fufaa — safety net dabalataa
