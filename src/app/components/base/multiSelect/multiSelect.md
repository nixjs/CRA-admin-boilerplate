### `MultiSelect` component

#### 🚀 usage:

    const  arrayDATA  = [
    		{ name: 'Vue.js', language: 'JavaScript' },
    		{ name: 'Rails', language: 'Ruby' },
    		{ name: 'Sinatra', language: 'Ruby' },
    		{ name: 'Laravel', language: 'PHP' },
    		{ name: 'Phoenix', language: 'Elixir' },
    ];

    <MultiSelect label="name" trackBy="name"  options={arrayDATA} onGetValues={onGetValues}  />

#### 🚀 props:

| **Name**          | **Type**              | **Default**                                            | **Description**                                                                                                            |
| ----------------- | --------------------- | ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------- |
| **options**       | `Array`               | []                                                     | Array of available options: Objects, Strings or Integers. If array of objects, visible label will default to option.value. |
| **trackBy**       | `String`              | key                                                    | Used to compare objects.                                                                                                   |
| **label**         | `String`              | value                                                  | Label from option Object, that will be visible in the dropdown.                                                            |
| **value**         | `Array|String|Number` |                                                        | Presets the selected options.                                                                                              |
| **disabled**      | `Boolean`             | false                                                  | Allow / not allow select option.                                                                                           |
| **searchable**    | `Boolean`             | true                                                   | Add / removes search input.                                                                                                |
| **onGetValues**   | `Function`            |                                                        | Emitted after the select options.                                                                                          |
| **name**          | `String`              | mutilselect_input                                      | Name attribute to match optional search element.                                                                           |
| **placeholder**   | `String`              | Select option                                          | Equivalent to the placeholder attribute on a `<select>` input.                                                             |
| **selectLabel**   | `String`              | Press enter to select                                  | String to show when pointing to an option.                                                                                 |
| **selectedLabel** | `String`              | Selected                                               | String to show next to selected option.                                                                                    |
| **deselectLabel** | `String`              | Press enter to remove                                  | String to show when pointing to an already selected option.                                                                |
| **noOptions**     | `String`              | List is empty.                                         | Shows when no elements in options empty. Default: List is empty.                                                           |
| **noResult**      | `String`              | No elements found. Consider changing the search query. | Shows when no elements match the search query.                                                                             |