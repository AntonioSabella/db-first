<!-- Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario -->

# Dealership

## Model: Car

## table: Cars

- id :                   BIGINT                PRIMARY KEY, UNIQUE, AUTO_INCREMENT, NOTNULL
- brand_name :           VARCHAR(30)           NOTNULL, INDEX
- model :                VARCHAR(30)           NOTNULL, INDEX
- car_image :            VARCHAR(255)          NULL
- matriculation_year :   YEAR(YYYY)            NULL
- mileage :              MEDIUMINT             NOTNULL
- price :                DECIMAL(8,2)999999.99 NULL
- discount :             TINYINT(t/f - 1/0)    NULL
- discount_value :       DECIMAL(7,2)999999.99 NOTNULL
- financing :            TINYINT(t/f - 1/0)    NULL
- monthly_rate:          DECIMAL(5, 2) 999.99  NULL
- conditions :           VARCHAR(15)           NULL
- color :                VARCHAR(25)           NOTNULL
- optionals :            TINYINT(t/f - 1/0)    NULL
- optionals_description :TEXT                  NULL
- power_hP(horsePower) : SMALLINT              NULL
- cubic_capacity :       SMALLINT              NULL
- doors_number :         TINYINT               NULL
- seats_number :         TINYINT               NULL
- previous_owners :      VARCHAR(50)           NULL
- damaged :              TINYINT(t/f - 1/0)    NULL
- damage_description :   TEXT                  NULL
- original_engine :      TINYINT(t/f - 1/0)    NULL 
- testing_certificate :  TINYINT(t/f - 1/0)    NULL
- testing_validity :     TIMESTAMP             NULL
- warranty :             TINYINT(t/f - 1/0)    NULL
- years_warranty :       TINYINT               NULL
- vehicle_fuel :         VARCHAR(15)           NULL
- emission_class :       TINYINT               NULL
- database_insertion :   DATE                  DEFAULT (insertion db date)