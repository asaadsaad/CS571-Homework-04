# CS571 Homework 04
## Question 01
Create a custom hook `useForm` that will persist the state of all form controls in a single object:
```javascript
const App = () => {
  const [formValues, handleChange] = useForm({ email: "", password: "" });

  return (
    <div>
      <input
        name="email"
        placeholder="email"
        value={formValues.email}
        onChange={handleChange}
      />
      <input
        type="password"
        name="password"
        placeholder="password"
        value={formValues.password}
        onChange={handleChange}
      />
    </div>
  );
};
```
  
## Question 02
1. Convert Homework 03 (Calculator App) and persist the state by using `useReducer()`. Maintain a pure Reducer function.
2. Lift up the state to be global using `useContext()`. Do not provide `dispatch()` method, but instead pass helper functions.
